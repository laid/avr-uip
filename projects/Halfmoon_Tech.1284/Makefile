#Chip choice
MCU	= atmega1284p
CHIP	= m1284p

#Project name
NAME    = halfmoon_tech


HTTPD_FS_DIRNAME = httpd-fs-halfmoon_tech.1284

#Compiled apps
APPS  = port_app_mapper
APPS += webserver.PROGMEM
APPS += telnetd 
APPS += dhcpc 
#APPS += ntpclient
APPS += resolv
APPS += webclient.PROGMEM

#Compiled drivers
DEVS	+= enc28j60.tux #The rest are determined by makefiles for apps

#Compiled libs
#LIBS	+= misc 1wire analog eeprom uart 
LIBS += net_conf
LIBS += prod_conf
#LIBS += ee24xx

#Project specific files
$(NAME)_SOURCES = main.c clock-arch.c uart.c webclient_data.c
#$(NAME)_SOURCES += process_command.c


#Include global configurations
-include ../../MakeConf.include

#Include the genetic makefile
-include ../../Makefile.include

