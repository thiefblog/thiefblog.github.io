---
title: Ubuntu Nvidia Driver
tags: Nvidia, Drvier
categories: Ubuntu
---

# Ubuntu install Nvidia Driver

- 新增repository、update、裝driver

	sudo add-apt-repository ppa:graphics-drivers/ppa

	sudo apt update

	sudo apt install ubuntu-drivers-common

- 查詢建議及安裝驅動程式

	ubuntu-drivers devices

	third-party free recommended

	sudo apt install nvidia-driver-430

	sudo reboot

- 驅動程式基本資訊

	lsmod&#124;grep nvidia

[15fa 網路卡驅動](https://www.intel.com/content/www/us/en/download/14611/15817/intel-network-adapter-driver-for-pcie-intel-gigabit-ethernet-network-connections-under-linux.html? "15fa 網路卡驅動")

- 安裝網路卡驅動程式

	tar -xvf e1000e-3.8.4.tar.gz

	cd e1000e-3.8.4/src/

	sudo make install

	sudo reboot