<h2>Working with shell</h2>

* Linux shell allows interaction between the user and the operating system
* In linux shell, the first thing is the home directory that allows users to store files and folders
  - Example: `/home/Ifeanyi = Ifeanyi's home directory`
 * In command line (CLI) the tilde `~` represents the home directory


 <h3>Commands and Arguements</h3>

 * Some commands requires areguemnts to work, others do not.
   - Example: `echo` won't print anything unless you add an arguemnt
 
   ```bash
   echo "hello" 

   ``` 
   
   - Also commands like `uptime` do not require an arguemnt.

 Some commnands also requires a flag, example: to print hello without the trailing line afterwards, use `echo -n hello`


 <h2>Basic linux commands</h2>

* To create multiple directories; use mkdir and the names of the directories with spaces in between
  - Example: 

  ```bash
  mkdir Asia Africa Europe America
  ```

* To create a directory inside a directory, simply change to the directory where new directory will be created first
  - Example: `cd Africa and then mkdir Nigeria`
    * You can also decide to make a directory inside Nigeria: `mkdir Nigeria/Lagos`
    * create `Lagos` where the directory `Nigeria` is not yet available. This command will create both the directory Nigeria and Lagos but Lagos inside Nigeria directory: `mkdir -p Nigeria/Lagos`
* To rename a directory use the mv (move) command
  - Example: 

   ```bash
   mv /home/Ifeanyi/Africa/Nigeria/Lago /home/Ifeanyi/Africa/Nigeria/Lagos
   # Also to move a directory to a different location use mv command
   mv /home/Ifeanyi/Africa/USA /home/Ifeanyi/America/
   ```

 * The `touch` command is used to create a file, example: `touch /home/Ifeanyi/Africa/Nigeria/Lagos/ barbeach.txt`


 <h2>Command-line help</h2>

* Using command line to get help. Example: `whatis` - this is good if you do not know what a command does before using it.
* Another one is man the produces what a certain command is used for in details, eg. `man date`; gives you details about date.
* Also to search for specific keywords use the command aprops followed by the keyword. Example apropos Ifeanyi will search for all the occurences of Ifeanyi.

Next up will be types of shells

<h2>Types of shell</h2>

* Bourne Shell (sh) 
* C Shell (csh or tcsh) 
* Korn Shell (ksh) 
* Z Shell (zsh) 
* Bourne again Shell (ba    sh).

* to know the type of shell you are working on, use `echo $SHELL`

* Use aliases to shorten commands: That's assigning a variable to a command. Example `ga=git add`, instead of typing `git add`, users can easily type `ga`. To set an alias called `up` for the command `uptime` and make it persistent to `~/.profile`. Use the command `alias up=uptime` and `'echo alias up=uptime'` `>> ~Ifeanyi/.profile`

<h3>Path variable</h3>
* The command `echo $PATH` prints your path
* To use the which command, you have to first export the path:`export PATH=$PATH:/opt/obs/bin` and then use the which command; example: `which obs-studio'
