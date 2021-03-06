ORADOCLETPLUS
=============

 * Copyright (C) 2010 Vladimir Katchourovski & Richard Nichols
 *
 * This program is free software; you can redistribute it and/or
 * modify it under the terms of the GNU General Public License
 * as published by the Free Software Foundation; either version 2
 * of the License, or (at your option) any later version.
 *
 * This program is distributed in the hope that it will be useful,
 * but WITHOUT ANY WARRANTY; without even the implied warranty of
 * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 * GNU General Public License for more details.
 *
 * You should have received a copy of the GNU General Public License
 * along with this program; if not, write to the Free Software
 * Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.

What is it?
-----------

OraDocletPlus is an enhanced version of the OraDoclet database documentation generator available at http://oradoclet.sourceforge.net/

The tool will automatically generate a set of HTML documents based on the Oracle database schema that you connect it to. It will pull our pretty much all meta-data about the schema, including indexes, column comments, foreign keys, and PL/SQL source code.

I threw these changes together as I needed to generate some database schema documentation quickly and found the original OraDoclet to be a pretty good solution, although it had a couple of bugs, looked very out of date and hasn’t been updated in quite a while.

Note that the original author of OraDoclet was Vladimir Katchourovski – kudos to him for creating a concise & simple tool.


Usage
-----

java -jar oradocletplus.jar username/password@hostname:port:sid &lt;output_directory> [&lt;copyright_notice>]

for example - 

java -jar oradocletplus.jar fred/password@localhost:1521:mydb c:/temp/oradocs "My Company Inc."
