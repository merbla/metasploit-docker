FROM ubuntu:trusty
RUN apt-get -qq update
RUN apt-get install -y wget curl

RUN curl https://raw.githubusercontent.com/rapid7/metasploit-omnibus/master/config/templates/metasploit-framework-wrappers/msfupdate.erb > msfinstall && chmod 755 msfinstall && ./msfinstall

CMD msfconsole