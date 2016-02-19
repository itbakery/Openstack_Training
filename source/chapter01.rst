บทที่ 1 เตรียมความพร้อม
####################

.. note:: ติดตั้งโปรแกรม

ติดตั้ง Virtualbox
****************
.. code-block:: bash
   :linenos:

   su -
   # Add repo
   cd /etc/yum.repos.d/
   wget http://download.virtualbox.org/virtualbox/rpm/rhel/virtualbox.repo

   # Install epel-repo
   yum install epel-release
   yum groupinstall "Development Tools"
   yum install binutils gcc make patch libgomp glibc-headers glibc-devel kernel-headers kernel-devel dkms

   yum install VirtualBox-5.0
   service vboxdrv setup
   usermod -a -G vboxusers `whoami`
   reboot


ติดตั้ง kvm
*********

ติดตั้ง Livert
===========
