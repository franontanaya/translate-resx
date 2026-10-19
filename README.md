# translate-resx
Terminal command to translate .resx format files using common translate services.

Mainly intended for translating Gruntz localization files. {TAG} placeholders are escaped so they aren't translated. 

## Usage:
./translate-resx -i /path/to/inputfile.resx -l targetlanguagecode

Copy to ~/bin to call it anywhere without ./

The current version of your file will be backed up to timestamp_filename.bak. The input file will be overwritten with the changes.

## Requirements
Requires any Linux install with the required packages.

Requires the CLI PHP interpreter
On debian based linux, install with "sudo apt install php-cli"

Uses the SimpleXML extension for PHP.
On debian based linux, install with "sudo apt install php-xml" 

Uses translate-shell to send the translation requests
On debian based linux, install with "sudo apt install translate-shell"
