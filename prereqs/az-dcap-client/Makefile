# Copyright (c) Microsoft Corporation. All rights reserved.
# Licensed under the MIT License.

all: setuprepo

setuprepo:
	echo "deb [arch=amd64] https://packages.microsoft.com/ubuntu/16.04/prod xenial main" | sudo tee /etc/apt/sources.list.d/msprod.list
	wget -qO - https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -

clean:

install:
	sudo apt-get install -y az-dcap-client

uninstall:
	sudo apt-get --purge remove az-dcap-client

