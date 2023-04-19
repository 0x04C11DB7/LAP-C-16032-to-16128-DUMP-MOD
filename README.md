# LAP-C-16032-to-16128-DUMP-MOD
LAP-C 16032 Dump Backup + Modified Dump from 16032 to 16128

EEPROM 93LC46B (64x16bit)

from zeroprog (https://github.com/t-bucchi/zeroprog):

  CRC = 0xFF00 | ((VID >> 8) + (VID & 0xFF) + (PID >> 8) + (PID & 0xFF) + 1);
  
#define OFFSET_VID			      0
#define OFFSET_PID			 1
#define OFFSET_CRC				2
#define OFFSET_MANUFACTURER		8
#define OFFSET_MODEL			0x20
#define OFFSET_SERIAL			0x38
	
	LAP-C(16032)	==>		VID: 0x0C12, PID: 0x700E, CRC: 0xFF9D
	LAP-C(16064)	==>		VID: 0x0C12, PID: 0x7009, CRC:
	LAP-C(16128)	==>		VID: 0x0C12, PID: 0x700A, CRC: 0xFF99
	LAP-C(162000)	==>		VID: 0x0C12, PID: 0x7016, CRC:

	LAP-C(32128)	==>		VID: 0x0C12, PID: 0x700B, CRC:
	LAP-C(321000)	==>		VID: 0x0C12, PID: 0x700C, CRC:
	LAP-C(322000)	==>		VID: 0x0C12, PID: 0x700D, CRC:
  
  
LAP-C(16032) DUMP:
  
  00000000  120C 0E70 9DFF FFFF FFFF FFFF FFFF FFFF  ...pќяяяяяяяяяяя
  00000020  1B5A 4552 4F50 4C55 5320 5465 6368 6E6F  .ZEROPLUS Techno
  00000040  6C6F 6779 2043 4F2C 2E4C 5444 FFFF FFFF  logy CO,.LTDяяяя
  00000060  FFFF FFFF FFFF FFFF FFFF FFFF FFFF FFFF  яяяяяяяяяяяяяяяя
  00000100  245A 4552 4F50 4C55 5320 4C6F 6769 6320  $ZEROPLUS Logic 
  00000120  416E 616C 797A 6572 284C 4150 2D43 2D31  Analyzer(LAP-C-1
  00000140  3630 3332 29FF FFFF FFFF FFFF FFFF FFFF  6032)яяяяяяяяяяя
  00000160  0F30 3030 3032 3030 3931 5A2D 3031 3230  .000020091Z-0120
  
  
LAP-C(16128) DUMP:

  00000000  120C 0A70 99FF FFFF FFFF FFFF FFFF FFFF  ...p™яяяяяяяяяяя
  00000010  1B5A 4552 4F50 4C55 5320 5465 6368 6E6F  .ZEROPLUS Techno
  00000020  6C6F 6779 2043 4F2C 2E4C 5444 FFFF FFFF  logy CO,.LTDяяяя
  00000030  FFFF FFFF FFFF FFFF FFFF FFFF FFFF FFFF  яяяяяяяяяяяяяяяя
  00000040  245A 4552 4F50 4C55 5320 4C6F 6769 6320  $ZEROPLUS Logic 
  00000050  416E 616C 797A 6572 284C 4150 2D43 2D31  Analyzer(LAP-C-1
  00000060  3631 3238 29FF FFFF FFFF FFFF FFFF FFFF  6128)яяяяяяяяяяя
  00000070  0F30 3030 3032 3030 3931 5A2D 3031 3230  .000020091Z-0120
  
