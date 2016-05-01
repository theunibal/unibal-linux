# UniBal Keyboard Layout for Linux

Installation Instructions (Advanced)
---

cd unibal-linux-master
sudo cp baL /usr/share/X11/xkb/symbols

sudo gedit /usr/share/X11/xkb/rules/evdev.xml
add this before `</layoutList>`

```xml
<layout>
	<configItem>
		<name>bal</name>
		<shortDescription>bal</shortDescription>
		<description>Baluchi</description>
		<languageList>
			<iso639Id>bal</iso639Id>
		</languageList>
	</configItem>
	<variantList/>
</layout>
```

- Save it
- Log Out and Log back in
- Open terminal and type:
    - `unity-control-center keyboard`
- Click `Text Entry`
- From below the `Input sources to use` click the plus button and search for `bal` click `Add`
- Now you can switch to the Balochi keyboard from the system tray. 

