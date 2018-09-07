# Violetto
Themes & configuration tip to get a clean linux system

This is a general guideline which involves modifying many system components. 
For reference on how to do single things, check [my website](https://fraanz.github.io/) 
or the [gentoo wiki](https://wiki.gentoo.org). The purpose is achieving simplicity 
and removing everything that can distract you from your job.

### Section 0: the boot process
 * If you can, disable bios debug messages (and intel subliminal logo XD)
 * If you are using grub, try using the theme included in this repo. To install it, 
   type in a shell:
   ```bash
   sudo cp grub-theme.txt /boot/grub/themes/violetto.txt
   # At this point you have to enable it in your /etc/default/grub
   sudo nano /etc/default/grub
   # Then regenerate the config file
   sudo grub-mkconfig -o /boot/grub/grub.cfg
   ```
 * Disable non-critical kernel and init messages
 * Configure your display manager to use a minimalist theme

### Section 1: desktop environment
If you followed correctly the previous instruction, you should have a beautiful, 
minimal, boot process. Now we have to configure the working space.

 * Try to start with a minimal window manager. Remove everything from the screen.
 * Use a solid dark background (or other colors but beware of their effects on 
   your mind... not kidding, every color has its own effects!)
 * Desktop bar and windows titles are useful, but configure them in order to have
   only the bare minimum to get your work done
  
### Section 2: software choice
This is the hardest part... I'm still working on it. As general guideline, terminal 
software should have less clutter than graphical equivalents... but I'm not sure 
however. You can start by choosing a modern minimal gtk/qt theme + icon set. Fonts 
also should be easy to read.

I'm testing this configuration to see if it works for me. Have you made any 
progress in the fight to mental fuzziness caused by bad interfaces? Remember to 
make a pull request or write me an email if you have any suggestions!

## Contacts

 * [Mail](fr4nz@protonmail.ch) 
 * [GitHub](https://github.com/fraanz)
