Documentation Contents

Official Web Site http://beewatch.de/waagen/stockwaagen/beewatch-professional/

Bluetooth
	Bluetooth parity code 1234
	(Check COM configuration, it could be an SPP profile)
	Recomended software:
		HTERM: http://www.der-hammer.info/terminal/ (Windows)
		Tera Term https://ttssh2.osdn.jp/index.html.en (Windows)
		https://play.google.com/store/apps/details?id=de.kai_morich.serial_bluetooth_terminal&hl=es-419 (Android)
		

Serial configuration
	Baudrate     -> 115200
	Data bits    -> 8
	Stop bits    -> 1
	Paarity      -> None
	Flow control -> None
	

LOGIN=3967  -------> Security code for 45726281 (Check security codes)

Commands that are not in the manual:
	RTCT=hh:mm:ss   -----> Establish hour
	RTCD=DD.MM.YY   -----> Establish date
	SETCFG          -----> Save configuration
	RTC             -----> Check current date and hour
	ALLP		-----> List configuration
	SETCFG		-----> Save changes in configuration
	Config;WINT=    -----> Establish taking lectures frequency (Seconds)
	STATE		-----> Scale current state, if "WAIT FOR WEIGHT", "READY" or "SIM ERROR" is ready to take lectures
	GET		-----> Retrive all lectures in the memory
		GET=#   -----> # Specify lectures of the number of days
	READ		-----> Retrieve one specific lecture (third element in weight).  