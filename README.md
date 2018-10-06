function onAnimation() {
		var str = "I've just read your bid in pleasant. This is a sample what you require. You will be fine, if you hire me.";
		if( pos == 0 )
			document.getElementById("conTxt").focus();
		if( pos == str.length ) {
			document.getElementById("conTxt").value = "";
			pos = 0;
		}
		var chr = str.substring(pos, pos+1);
		pos++;
		document.getElementById("conTxt").value += chr;
		setTimeout(onAnimation, 100);
	}
