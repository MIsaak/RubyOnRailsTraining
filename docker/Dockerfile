FROM ruby:3.0.6


RUN apt update && apt install -y zsh curl git vim

#Install Node.js 16
RUN curl -sL https://deb.nodesource.com/setup_16.x | bash -
RUN apt -y install nodejs

RUN sh -c "$(wget https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"

# Set the default shell to zsh rather than sh
RUN chsh -s $(which zsh) $(whoami) 

RUN gem install rails