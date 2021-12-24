FROM circleci/ruby:2.5.1-stretch-node-browsers

RUN sudo apt-get install curl ca-certificates gnupg
RUN curl https://www.postgresql.org/media/keys/ACCC4CF8.asc | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/apt.postgresql.org.gpg >/dev/null
RUN sudo bash -c 'echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main" >> /etc/apt/sources.list.d/pgdg.list'
RUN sudo apt-get update
RUN sudo apt-get -y --allow-unauthenticated install postgresql-client-9.5
