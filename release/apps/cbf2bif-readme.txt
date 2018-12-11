=========================================================================================

 README & LICENSE

 CBF2BIF v1.0.0.0 (18.01.2011) by fearless

 Copyright (c) 2013 www.LetTheLight.in

 All Rights Reserved

 fearless.is.my.name@gmail.com
 fearless@letthelight.in
 www.LetTheLight.in


 This software is provided 'as-is', without any express or implied warranty. In no
 event will the author be held liable for any damages arising from the use of this
 software.

 Permission is granted to anyone to use this software for any non-commercial program.
 If you use the library in an application, an acknowledgement in the application or
 documentation is appreciated but not required. 

 You are allowed to make modifications to the source code, but you must leave the
 original copyright notices intact and not mispresent the origin of the software.
 It is not allowed to claim you wrote the original software. Modified files must have
 a clear notice that the files are modified, and not in the original state. This includes
 the name of the person(s) who modified the code. 

 If you want to distribute or redistribute any portion of this package, you will need
 to include the full package in it's original state, including this license and all
 the copyrights. 

 While distributing this package (in it's original state) is allowed, it is not allowed
 to charge anything for this. You may not sell or include the package in any commercial
 package without having permission of the author. Neither is it allowed to redistribute
 any of the package's components with commercial applications.

=========================================================================================



=========================================================================================
 About
=========================================================================================

 CBF2BIF is a utility to uncompress infinity engine bif format files. These file types 
 are commonly found in the following games:

 - Baldurs Gate
 - Baldurs Gate: Tales of The Sword Coast
 - Baldurs Gate II: Shadows of Amn
 - Baldurs Gate II: Throne of Bhaal
 - Icewind Dale
 - Icewind Dale: Trials of the Luremaster
 - Icewind Dale: Heart of Winter
 - Icewind Dale II
 - Planescape Torment


 Features:

  - Decompression of BIF V1.0 and BIFC V1.0 compressed BIF file formats.
  - Supports * and ? wildcards for batch operations
  - Optionally can specify filename to decompress a single specified file to 
    (wildcards are not supported in this operation)


 Notes: 

 !!! CBF2BIF IS A CONSOLE MODE PROGRAM AND MUST BE RAN FROM A COMMAND PROMPT !!!

 If destination filename is not specified, the output is to the original input filename 
 provided, overwritting the original file data, except in the case of CBF/BIF V1.0 files,
 in which case the output is to the filename which is stored internally in the CBF/BIF 
 container.

 If you wish to prevent accidentally overwritting files, specify both source input
 filename and destination output filename. The internal filename in the CBF/BIF container 
 files will be ignored in this case.


=========================================================================================
 Credits
=========================================================================================

 Copyright (C) 2013 ƒearless - LetTheLightIn

 Whilst some of the functions in this tool have been written by myself, contributions 
 from other sources have helped in its development.

 Credit belongs to the following people and resources used in this tool, for ideas, code 
 and/or algorithms that have been derived or adapted from their original submissions:


 Source/Author                    Info               Webpage
-----------------------------------------------------------------------------------------
 Ketil “KetilO” Olsen             RadASM IDE         http://radasm.cherrytree.at/	
 Steve Hutch                      MASM32 libraries   http://www.masm32.com
 Jean-loup Gailly and Mark Adler  Zlib Library       http://www.zlib.net
 IE Modding Communities           IESDP              http://iesdp.gibberlings3.net	


 A big thank you to all Infinity Engine modders who have helped document the internals of 
 the Infinity Engine and to compile the fantastic resource of The Infinity Engine 
 Structures Description Project (IESDP) hosted currently at:

 http://iesdp.gibberlings3.net




