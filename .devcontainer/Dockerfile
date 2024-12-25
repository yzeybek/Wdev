FROM yzeybek/beroot

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get -y update && apt-get -y upgrade

RUN pipx install norminette && pipx ensurepath && \
	python3 -m pip config set global.break-system-packages true && \
	pip3 install c_formatter_42 && \
	bash -c "$(curl -fsSL https://raw.github.com/xicodomingues/francinette/master/bin/install.sh)"
