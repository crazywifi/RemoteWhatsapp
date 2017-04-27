REMOTE WHATSAPP
Q1. what is this application?
This script is whatsapp script that use python.it is made by Tarek Galal
<tare2.galal@gmail.com> MIT License.name is yowsup-master .
I modified this script and name it REMOTE WHATSAPP .In this script I add some
module that help administrator or normal user to control linux os by whatsapp only by
sending command.it is a beta version.

Q2. module added by me?
1. Shutdown: u can shut down by sending command Shutdown.
2. Restart: u can restart by sending command Restart.
3. Suspend:u can suspend by sending command Suspend.
4. Screenshot:u can take screenshot by sending command Screenshot.
5. Screenshot50:u can take screenshot by sending command Screenshot50.it take
50 screenshot continuouslt in 5 sec gap.
6. Screenlock: u can screenllock by sending command shutdown.
7. Keylogger: u can install keylogger.it can monitor your laptop when other one
using it. u not at home and some one using it u only send command and start
keylogger.

Q3. how to setup whatsap?
1.download remote whatsapp folder in root directory.in this folder yowsup-master
folder copy it to root directory.
1. “install.sh” script is give in the remote whatsapp folder.make it executable
Chmod +x install.sh
2. run this script and install dependencies.
./install.sh
3.cd yowsup-master/src
4.nano config.example
here u find this
cc=91
phone=91your mobile number to register for whatsap<no. With no whatsap>
id=
password=
5.chmod +x yowsup-cli
6. ./yowsup-cli --requestcode sms --config config.example
u get something like this:
status:sent
length:6
method:sms
7. u get a code in your number u give above..it is like u register for whatsap in your
phone
./yowsup-cli --register 123-456 --config config.example

8.now u get password on your screen.open another terminal go to /yowsup-master/src
and open config.example and type your password .
## Actual config starts below ##
cc=
phone=
id=
password= your password
9. your whatsapp now set up.
10. open run.sh script and in other number place write the number from which u can
send your command.

Q4. how to configure KEYLOGGER??
I use logkeys-0.1.1 as a keylogger. Logkeys is a Linux keylogger. It is more updated
than any other available keylogger, Moreover logkeys don’t crash the X server, and
appears to work in all the situations. Logkeys creates a log of all characters and
function keys. Moreover logkeys are aware of Alt and Shift and works
well with serial as well as USB keyboards.
1. extract logkeys
tar -xvzf logkeys-0.1.1a.tar.gz
2. go to logkeys folder
cd logkeys-0.1.1a
3. ./configure
4. make
5. sudo make install
6. sudo locale-gen
Usages of logkeys:
logkeys s : Start logging keypress.
logkeys k : Kill logkeys process.
Check the log file which by default is ‘/var/log/logkeys.log‘.
nano /var/log/logkeys.log

Q5. how to start script automatically?
Open terminal and type
crontab -e
and at last type this.give run.sh script path here but before this it is important it run.sh is
executable.
@reboot /root/yowsup-master/src/run.sh

Q6. what command I can send from whatsapp and command working?
Shutdown
Restart
Suspend
Screenlock
this commands help you when you are away from your laptop. Let take a scenario u r not
at home and someone want your pc or use your pc or u download something..by sending
this command u can control your pc.more commands
Screenshot
Screenshot50
this commands help you to take screenshot when someone using your
laptop.Screenshot50 take 50 screenshot in 5sec interval.
All these screenshot save to /root/yowsup-master/src/.screenshot
Logkeys -s
this is a keylogger command to start keylogger .
Logkeys -k
this is a keylogger command to stop the keylogger.

Note: first letter is always capital of whatsapp command like Screenshot 'S' is
capital.otherwise not working.
Hope you like my work .this is beta version .i try to send reply and more feature to your
whatsapp..u can see power status and many more feature at your whatsapp.
RISHABH SHARMA
rishabh2241991@gmail.com


