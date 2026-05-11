# []Translate Sao Mai Braille
Below are steps to get started.
Note, if any of following steps you’re already done, please skip it.
For any question/request, please don’t hesitate to drop us a message at:
<support@saomaicenter.org>
(send e-mail).

## Preparation for translation
1. Download and install latest Sao Mai Braille from: 
<https://saomaicenter.org/en/smsoft/smb>.
By default, SMB is installed on system C drive, in: “C:\Program Files\SaoMai\SMB”
2. Download the SM Translator tool to manage your translation process at:
[SMTranslator.exe](https://saomaicenter.org/sites/default/files/inline-files/SMTranslator.exe).
It’s recommended to save it in a folder on a writable drive, such as in: “d:\SMB Translation”.
3. Fork this repository to your Github account, then download it to your computer.
4. Open the repository, navigate to smb/AvailableLanguages folder.
It has language files which are some fully translated and mostly partially translated.

### Important notes
- Language file extension is the three-letter defined for that language in ISO 639-3.
For instance: “SMB.eng” is for English. Check language code at:
<https://iso639-3.sil.org/code_tables/639/data>
- All UI language files are saved in “Lang” folder in the SMB’s installed folder.
You can paste the translated language file in this folder to see how it’s shown in Sao Mai Braille.
- It always has a pair of files: 1) the base file is the original English one (SMB.eng), and 2) the saved file as the target language to be translated.
This you can find in the “Available Languages” folder.
- Please keep your translated language and “SMB.ref” files in “d:\SMB Translation” folder for future update.
The translated language file generated in “D:\SMB Translation\Release” folder is used to check the result and sent to us to include in Sao Mai Braille.
- Special character “&” is used to define hotkeys in combination with “Alt” key for that feature.
So, you can remove it or move it right before the character in your translation language that you want to make it become the hotkey.
- Text with % sign like “%s” should be kept intact.
However, you can move it to other suitable position of the sentence in your language.
- Text in left/right brackets should be kept intact.

## Translate/improve existing UI language
You can open SMB, go to Tools and choose interface language to see if your language is available or not.
If it’s available, you can check and consider to translate new strings or improve existing ones.
1. Go to the “Available Languages” folder and copy “SMB.eng” base file and the language file that you want to improve.
Then, paste them in same folder with “SMTranslator.exe” tool in “D:\SMB Translation”.
For example: Norwegian language file should be “SMB.nor”; or for Italian is “SMB.ita” etc.
2. Run “SMTranslator.exe” and press Alt+o, choose language file to open to translate.
3. After opened, focus will be in a string list, where you can browse for string that you want to translate or improve.
 Press Tab once will be on English source string read-only field.
Tab again will be on edit field to improve or translate the string into your language.
Please note, press F2 to save every time finishing a string.
Or, esc to cancel.
4. Move back to the string list, repeat same steps to translate other strings.
 Please don’t forget to choose Save button or press alt+s to save the translation file.
5. There’s a checkbox to show only untranslated or all strings.
6. 6. When pressing Save button to save, it will confirm if you want to save the .REF file.
 Choose "Yes" to save it for future update and string comparison between the old and new ones.
7. To test how it’s written in SMB’s user interface, copy your target language file in “D:\SMB Translation\Release” folder, and replace the old one in “C:\Program Files\SaoMai\SMB\Lang”.
 Run SMB and choose your translated language.
8. When you’re satisfied with the translation, please commit to your  forked repository on Github, then make a pull-request so we'll get it.
 Or e-mail to us at: <support@saomaicenter.org>.
 We will pack it with next release.
 
 ## Translate new language
 1. Copy “SMB.eng” English base file from installed “Lang” folder, and paste it into “SMB Translation”.
 2. Run “SMTranslator.exe” tool and press Alt+n to create new language translation file.
 3. Choose English base file by pressing Browse... button, choose “SMB.eng” in the same “SMB Translation” folder with SM Translator tool. And fill following information and choose Ok.
     - English name: new language’s name in English.
    - Native name: language’s name written in its native language.
    - File extension: provide 3-letter file extension for this new language based on ISO639-3.
4. Move to list of strings and choose to translate.
Press Tab once will be on English source string read-only field.
Tab again will be on edit field to translate string into your language.
Please note, press F2 to save every time finishing a string.
Or, esc to cancel.
 5. Move back to the string list, repeat same steps to translate other strings.
 Please don’t forget to choose Save button or press alt+s to save the translation file.
 6. When pressing Save button to save, it will confirm if you want to save the .REF file.
 Choose "Yes" to save it for future update and string comparison between the old and new ones.
 7. To test how it’s written in SMB’s user interface, copy your target language file in “D:\SMB Translation\Release\” folder, and replace the old one in “C:\Program Files\SaoMai\SMB\Lang”.
 Run SMB and choose your translated language.
8. When you’re satisfied with the translation, please commit to your  forked repository on Github, then make a pull-request so we'll get it.
 Or e-mail to us at: <support@saomaicenter.org>.
 We will pack it with next release.
 
## Translating third-party components
We're using LibLouis library to convert literature text from print to Braille, and MathCAT to convert Math equations into Braille and speech.
Therefore, requests related to Braille translation table for text, we recommend to visit LibLouis library's website for more information:
<http://liblouis.org/>
And for Math equation conversion into Braille and speech, please visit MathCAT website at:
<https://github.com/NSoiffer/MathCAT>
However, you can contact us for any questions regarding to any issues and feature requests.