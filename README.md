# README

Lets first get your environment ready, follow the below-mentioned procedure:
(THIS IS FOR UBUNTU/Debian only)

1. Open terminal and run: sudo apt-get install ruby-full 
2. Installation of asdf, run these commands in shell:
    1. git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.9.0
    2. sudo gedit ~/.bashrc
    3. Go the bottom and paste these and save the file:
        1. . $HOME/.asdf/asdf.sh
        2. . $HOME/.asdf/completions/asdf.bash
3. Installation of postgresql, run these commands in shell:
    1. sudo apt-get install linux-headers-$(uname -r) build-essential libssl-dev libreadline-dev zlib1g-dev libcurl4-openssl-dev uuid-dev
    2. asdf plugin-add postgres
    3. asdf install postgres latest
    4. asdf postgres global latest
    5. createdb default
    6. psql -d default
    7. psql shell will open, there write this: CREATE USER postgres SUPERUSER WITH PASSWORD 'postgres'; for creating a superuser with username: postgres and password: postgres
4. Installation of node, run these commands in shell:
    1. asdf plugin-add nodejs
    2. asdf install nodejs latest
    3. asdf global nodejs latest
5. Installation of yarn: npm install --global yarn
6. Finally, install rails by: gem install rails
    
