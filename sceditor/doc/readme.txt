***** Written by Hiền Trung 
***** Develop for LiveHelperChat
***** Web: http://livehelperchat.com
***** Source: http://livehelperchat.com
---------------------------------------

Use SCEditor to replace textarea input chat for operator and visitor of module lhchat (not implement for chatbox)
Refer : http://www.sceditor.com/

	+ Add and fix some code to use for livehelperchat
	+ Edit default value config : toolbar, style, emoticon (from line 5319 of file jquery.sceditor.bbcode.js)
	+ Add option config : customizeToolbar, keyEnter, keyPress

Override : 
	+ Pagelayout for include css and js of sceditor
	+ Template chat and adminchat, replace textarea to sceditor (bbcode)
	+ Class lhBBCode, add some code convert BBCode for emoticon, color, strike
	+ Change lh.js, old version unbind textarea input, to new version is destroy sceditor object

Note: To add more emoticon, must declare in jquery sceditor, and then write code convert BBCode to html, folder images/smiley
has a lot of emoticon yahoo not use in editor
