# Ambiance Desktop

<img src="ambiance_D.png" width="160" border-effect="rounded" />

<tabs>

<tab id="ambiance_d" title="Ambiance Desktop">

<table>
    <tr>
        <td></td>
        <td>Table of Content</td>
    </tr>
    <tr>
        <td>1</td>
        <td><a href="#Installation">Install on Linux</a></td>
    </tr>
    <tr>
        <td>2</td>
        <td><a href="#QuickStart">Getting Started with Ambiance</a></td>
    </tr>
    <tr>
        <td>3</td>
        <td><a href="#DealingWithErrors">Dealing with Errors</a></td>
    </tr>
</table>



<chapter id="Installation" title="Installation">

<tip title="Linux Geek?">
<a href="#install-like-a-pro">Click to jump directly on Linux Installation like a pro!</a>
</tip>
<p>Installing Ambiance Desktop is one of the simplest tasks. <br/><br/> Thanks to its embedded graphics and backend engine, that works independent of your platform, provided that your platform can run that engine. <br/> Yes it works like java!</p>

<h5> As A Native App </h5>
<tabs>
<tab title="Ubuntu (.deb)">
<br/>

1. Download `ambiance_deb.tar.xz` from Download portion or [My Portfolio Site](https://snippetsofpassion.vercel.app/apps)
2. Extract the tarball package using Nautilus, or using CLI:
```Shell
cd Downloads # or location where you downloaded
tar -xf ambiance_deb.tar.gz
```
3. Run `install.sh`
```SHELL
cd ambiance
chmod +x ./install.sh && ./install.sh
```

</tab>
<tab title="Fedora (.rpm)"></tab>
</tabs>

<h5> OR use as AppImage [ Standalone ] </h5>
Just before you begin, know some facts about AppImage...
1. Stays in the form of a loose file
2. Requires manual navigation and running
3. Not indexed in app listing (generally)

Installation process:
1. Extract the package (as indicated above)
2. Open the extracted directory

<img src="ambiance_desktop_installation_1.png" width="400" />

3. Open properties of the AppImage (ambiance_desktop) : Usually <shortcut>Alt</shortcut> + <shortcut>Enter</shortcut>

<img src="ambiance_desktop_installation_2.png" alt="" width="400"/>

4. Ensure that it is `Executable as Program`
5. Now, just double click the AppImage and you are ready to go :)

<video src="Ambiance_Installed.webm" border-effect="rounded" mini-player="true" />

</chapter>


<chapter id="QuickStart" title="Getting Started"> 
As we know, Ambiance Desktop is derived from the android Ambiance app, it focuses on speedy and reliable key-value pairs.

<h4>Using shortcut keys for quick input</h4>
<p> As you can see on the end, when you type, the app suggests you to press the Tab and Enter key. </p>

1. <shortcut> Tab </shortcut> key to jump

<img src="ambiance_desktop_shortcutkey_1.png" style="block" border-effect="rounded" />
<p>When typing the title, you can hit <shortcut>Tab</shortcut> to jump to value</p>

2. <shortcut>Enter</shortcut> to save

<img src="ambiance_desktop_shortcutkey_2.png" style="block" border-effect="rounded" />
<p>When typing the value, you can hit <shortcut>Enter</shortcut> to save the pair</p>

</chapter>

<chapter id="DealingWithErrors" title="Dealing With Errors">
<chapter id="file-corruption" title="File Corruption">
<img src="ambiance_fileCorruption.png" width="500" />
<p>Most probably, a file corruption must look like this, or even worse...</p>
<p>There are 2 ways to fix the error:</p>
<h6> Method 1 </h6>

1. Navigate to app settings.
2. Click on `Clear My Data`.
![ambiance_fileCorruption_ClearMyData1.png](ambiance_fileCorruption_ClearMyData1.png)
<warning title="Caution">
This method truncates all your data PERMANENTLY
</warning>

<h6> Method 2 (advanced) </h6>

<br/>

1. Navigate to `/opt/ambiance` or your AppImage directory if you use AppImage.
2. Here you must find all your data in csv format. Open it.
![ambiance_fileCorruption_3.png](ambiance_fileCorruption_3.png)
3. Find out the line causing error
![ambiance_fileCorruption_5.png](ambiance_fileCorruption_5.png)
4. Here, clearly the first line doesn't have 2 members like others, just as a normal CSV should.
5. Manually fix this error, either remove or repair this line.
![ambiance_fileCorruption_6.png](ambiance_fileCorruption_6.png)
6. All done!
<img src="ambiance_fileCorruption_success.png" width="400" />

<tip title="Tip"> Sometimes it becomes tricky to find the error in large files.<br/> For this, we are working on inbuilt error fixing algorithms. You can opt in for automatic Data Resolver provided within the app, that tries to recover your data while fixing potential corruption on its own.</tip>
</chapter>

</chapter>

</tab>

<tab title="Download">

<chapter level="3" title="Direct Download">
<a href="https://snippetsofpassion.vercel.app/releases/ambiance_deb.tar.xz">
Click this link to fetch from my portfolio
</a>
</chapter>

<chapter id="install-like-a-pro" level="3" title="Linux style">

1. Curl the tarball
```Shell
curl https://snippetsofpassion.vercel.app/releases/ambiance_deb.tar.xz --output ambiance-desktop.tar.xz
```

2. Extract the tarball
```Shell
tar -xf ./ambiance-desktop.tar.xz
```

3. Navigate to the extracted directory
```Shell
cd 'Ambiance Desktop'
```

4. If you want portable binary file, select `Potable AppImage` below, else carry on with Normal Install

<tabs>
<tab title="Normal">
<br/>

1. Run the install.sh script and let it do everything for you :)
```Shell
chmod +x ./install.sh && bash ./install.sh
```

</tab>
<tab title="Portable AppImage">
<br/>

1. Change AppImage's mode to Executable

```Shell
chmod +x ambiance_desktop
```
<br/>

2. Run the app

```Shell
./ambiance_desktop
```
</tab>
</tabs>
</chapter>

</tab>
</tabs>
