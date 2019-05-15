- `df`: the amount of free space on the disk drives
- `free`: the amount of free memory
- 结束一个终端会话
    - 关闭终端模拟器窗口
    - `ctrl-d`
    - `exit`
- `date`, `cal` (calendar)
# Shell
- Command line refers to the **shell**
- The shell is a program that takes keyboard commands and passes them to the operating system to carry out
- Almost all Linux distributions supply a shell program from the GNU Project called `bash`
    - `bash` is an acronym for *bourne-again shell*, a reference to the fact that `bash` is an enhanced replacement for `sh`, the original Unix shell program written by Steve Bourne
- When using a graphical user interface (**GUI**, like KDE, GNOME), we need another program called a **terminal emulator** to interact with the shell
- **Shell prompt** will appear whenever the shell is ready to accept input
    - `username@machinename ` followed by the current working directory and a `$` or `#`
        - A hash mark (**#**) means the terminal session has superuser privileges. It means either we are logged in as the root user or we selected a terminal emulator that provides superuser (administrative) privileges
- Command history: up / down arrow
- Mice and focus
    - A mechanism built into the X Window System (the underlying engine that makes the GUI go) supports a quick copy-and-paste technique. If you highlight some text by holding down the left mouse button and dragging the mouse over it (or double-clicking a word), it is copied into **a buffer maintained by X**. Pressing the middle mouse button will cause the text to be pasted at the cursor location
    - Don’t be tempted to use `ctrl-C` and `ctrl-V` to perform copy and paste inside a terminal window. They don’t work. These control codes have different meanings to the shell and were assigned many years before the release of Microsoft Windows
    - > Your graphical desktop environment (most likely KDE or GNOME), in an effort to behave like Windows, probably has its focus policy set to “**click to focus**.” This means for a window to get focus (become active), you need to click on it. This is contrary to the traditional X behavior of “focus follows mouse,” which means that a window gets focus just by passing the mouse ***over*** it. The window will not come to the foreground until you click on it, but it will be able to receive input. Setting the focus policy to “**focus follows mouse**” will make the copy-and-paste technique even more useful. Give it a try if you can (some desktop environments such as Ubuntu’s Unity no longer support it). I think if you give it a chance, you will prefer it. You will find this setting in the configuration program for your window manager
- Console behind the curtain
    - Even if we have no terminal emulator running, several terminal **sessions** continue to run behind the graphical desktop. We can access these sessions, called *virtual consoles*, by pressing `ctrl-alt-F1` through `ctrl-alt-F6` on most Linux distributions
    - When a session is accessed, it presents a login prompt into which we can enter our username and password. To switch from one virtual console to another, press `alt-F1` through `alt-F6`
    - On most systems, we can return to the graphical desktop by pressing `alt-F7`