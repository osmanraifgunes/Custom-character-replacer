# Custom-character-replacer
Relace non-latin characters to latin equivalent in a string

There are special characters (Ậ, Ş, Æ, Ť, Ü) used in some languages In some alphabets like Vietnamese, Turkish,etc.

Moreover, there are special characters inside string like ®, {, %, etc.

I used this to generate seo-friendly url from text. This script may be used for some special operations like clear text before printibg, seo, search text , etc.

Used sources to identify characters are :

http://graphemica.com/

https://www.compart.com/en/unicode/category

https://www.wikipedia.org/


CREATE FUNCTION [dbo].[ReplaceSeoCharacters]
(
	@StringValue NVARCHAR(MAX)
)
RETURNS NVARCHAR(MAX)
AS
BEGIN

	--Upper Case
	SET @StringValue = REPLACE(@StringValue,N'Ậ','A');
	SET @StringValue = REPLACE(@StringValue,N'Ấ','A');
	SET @StringValue = REPLACE(@StringValue,N'Ắ','A');
	SET @StringValue = REPLACE(@StringValue,N'Ặ','A');
	SET @StringValue = REPLACE(@StringValue,N'Ạ','A');
	SET @StringValue = REPLACE(@StringValue,N'Ả','A');
	SET @StringValue = REPLACE(@StringValue,N'Ầ','A');
	SET @StringValue = REPLACE(@StringValue,N'Ǟ','A');
	SET @StringValue = REPLACE(@StringValue,N'À','A');
	SET @StringValue = REPLACE(@StringValue,N'Ą','A');
	SET @StringValue = REPLACE(@StringValue,N'Ằ','A');
	SET @StringValue = REPLACE(@StringValue,N'Ă','A');
	SET @StringValue = REPLACE(@StringValue,N'Ā','A');
	SET @StringValue = REPLACE(@StringValue,N'Ẫ','A');
	SET @StringValue = REPLACE(@StringValue,N'Ẵ','A');
	SET @StringValue = REPLACE(@StringValue,N'Ẩ','A');
	SET @StringValue = REPLACE(@StringValue,N'Ẳ','A');
	SET @StringValue = REPLACE(@StringValue,N'Á','A');
	SET @StringValue = REPLACE(@StringValue,N'Â','A');
	SET @StringValue = REPLACE(@StringValue,N'Ã','A');
	SET @StringValue = REPLACE(@StringValue,N'Ä','A');
	SET @StringValue = REPLACE(@StringValue,N'Å','A');
	SET @StringValue = REPLACE(@StringValue,N'Æ','AE');
	SET @StringValue = REPLACE(@StringValue,N'Ɓ','B');
	SET @StringValue = REPLACE(@StringValue,N'Ƃ','B');
	SET @StringValue = REPLACE(@StringValue,N'Ƅ','B');
	SET @StringValue = REPLACE(@StringValue,N'Ċ','C');
	SET @StringValue = REPLACE(@StringValue,N'Ĉ','C');
	SET @StringValue = REPLACE(@StringValue,N'Ç','C');
	SET @StringValue = REPLACE(@StringValue,N'Č','C');
	SET @StringValue = REPLACE(@StringValue,N'Ć','C');
	SET @StringValue = REPLACE(@StringValue,N'Ɔ','C');
	SET @StringValue = REPLACE(@StringValue,N'Ƈ','C');
	SET @StringValue = REPLACE(@StringValue,N'Ɗ','D');
	SET @StringValue = REPLACE(@StringValue,N'₫','D');
	SET @StringValue = REPLACE(@StringValue,N'Ď','D');
	SET @StringValue = REPLACE(@StringValue,N'Ɖ','D');
	SET @StringValue = REPLACE(@StringValue,N'Đ','D');
	SET @StringValue = REPLACE(@StringValue,N'Ð','D');
	SET @StringValue = REPLACE(@StringValue,N'Ƌ','D');
	SET @StringValue = REPLACE(@StringValue,N'Ě','E');
	SET @StringValue = REPLACE(@StringValue,N'Ề','E');
	SET @StringValue = REPLACE(@StringValue,N'Ǝ','E');
	SET @StringValue = REPLACE(@StringValue,N'Ę','E');
	SET @StringValue = REPLACE(@StringValue,N'Ễ','E');
	SET @StringValue = REPLACE(@StringValue,N'Ė','E');
	SET @StringValue = REPLACE(@StringValue,N'È','E');
	SET @StringValue = REPLACE(@StringValue,N'Ệ','E');
	SET @StringValue = REPLACE(@StringValue,N'Ế','E');
	SET @StringValue = REPLACE(@StringValue,N'Ĕ','E');
	SET @StringValue = REPLACE(@StringValue,N'Ể','E');
	SET @StringValue = REPLACE(@StringValue,N'Ē','E');
	SET @StringValue = REPLACE(@StringValue,N'É','E');
	SET @StringValue = REPLACE(@StringValue,N'Ê','E');
	SET @StringValue = REPLACE(@StringValue,N'Ë','E');
	SET @StringValue = REPLACE(@StringValue,N'Ẽ','E');
	SET @StringValue = REPLACE(@StringValue,N'Ẻ','E');
	SET @StringValue = REPLACE(@StringValue,N'Ẹ','E');
	SET @StringValue = REPLACE(@StringValue,N'Ƒ','F');
	SET @StringValue = REPLACE(@StringValue,N'Ĝ','G');
	SET @StringValue = REPLACE(@StringValue,N'Ǥ','G');
	SET @StringValue = REPLACE(@StringValue,N'Ğ','G');
	SET @StringValue = REPLACE(@StringValue,N'Ġ','G');
	SET @StringValue = REPLACE(@StringValue,N'Ģ','G');
	SET @StringValue = REPLACE(@StringValue,N'Ɠ','G');
	SET @StringValue = REPLACE(@StringValue,N'Ǧ','G');
	SET @StringValue = REPLACE(@StringValue,N'Ƣ','G');
	SET @StringValue = REPLACE(@StringValue,N'Ḥ','H');
	SET @StringValue = REPLACE(@StringValue,N'Ĥ','H');
	SET @StringValue = REPLACE(@StringValue,N'Ħ','H');
	SET @StringValue = REPLACE(@StringValue,N'Ĭ','I');
	SET @StringValue = REPLACE(@StringValue,N'Ī','I');
	SET @StringValue = REPLACE(@StringValue,N'Ɩ','I');
	SET @StringValue = REPLACE(@StringValue,N'Ĩ','I');
	SET @StringValue = REPLACE(@StringValue,N'Ị','I');
	SET @StringValue = REPLACE(@StringValue,N'Ì','I');
	SET @StringValue = REPLACE(@StringValue,N'Ɨ','I');
	SET @StringValue = REPLACE(@StringValue,N'Í','I');
	SET @StringValue = REPLACE(@StringValue,N'Î','I');
	SET @StringValue = REPLACE(@StringValue,N'Ï','I');
	SET @StringValue = REPLACE(@StringValue,N'İ','I');
	SET @StringValue = REPLACE(@StringValue,N'Į','I');
	SET @StringValue = REPLACE(@StringValue,N'Ǐ','I');
	SET @StringValue = REPLACE(@StringValue,N'Ỉ','I');
	SET @StringValue = REPLACE(@StringValue,N'Ĳ','IJ');
	SET @StringValue = REPLACE(@StringValue,N'Ĵ','J');
	SET @StringValue = REPLACE(@StringValue,N'Ķ','K');
	SET @StringValue = REPLACE(@StringValue,N'Ǩ','K');
	SET @StringValue = REPLACE(@StringValue,N'Ƙ','K');
	SET @StringValue = REPLACE(@StringValue,N'Ĺ','L');
	SET @StringValue = REPLACE(@StringValue,N'Ļ','L');
	SET @StringValue = REPLACE(@StringValue,N'Ł','L');
	SET @StringValue = REPLACE(@StringValue,N'Ľ','L');
	SET @StringValue = REPLACE(@StringValue,N'Ŀ','L');
	SET @StringValue = REPLACE(@StringValue,N'Ñ','N');
	SET @StringValue = REPLACE(@StringValue,N'Ŏ','N');
	SET @StringValue = REPLACE(@StringValue,N'Ň','N');
	SET @StringValue = REPLACE(@StringValue,N'Ń','N');
	SET @StringValue = REPLACE(@StringValue,N'Ņ','N');
	SET @StringValue = REPLACE(@StringValue,N'Ŋ','N');
	SET @StringValue = REPLACE(@StringValue,N'Ɲ','N');
	SET @StringValue = REPLACE(@StringValue,N'Œ','OE');
	SET @StringValue = REPLACE(@StringValue,N'Ò','O');
	SET @StringValue = REPLACE(@StringValue,N'Ó','O');
	SET @StringValue = REPLACE(@StringValue,N'Ợ','O');
	SET @StringValue = REPLACE(@StringValue,N'Ờ','O');
	SET @StringValue = REPLACE(@StringValue,N'Ớ','O');
	SET @StringValue = REPLACE(@StringValue,N'Ō','O');
	SET @StringValue = REPLACE(@StringValue,N'Ố','O');
	SET @StringValue = REPLACE(@StringValue,N'Ő','O');
	SET @StringValue = REPLACE(@StringValue,N'Ồ','O');
	SET @StringValue = REPLACE(@StringValue,N'Ô','O');
	SET @StringValue = REPLACE(@StringValue,N'Õ','O');
	SET @StringValue = REPLACE(@StringValue,N'Ö','O');
	SET @StringValue = REPLACE(@StringValue,N'Ǒ','O');
	SET @StringValue = REPLACE(@StringValue,N'Ɵ','O');
	SET @StringValue = REPLACE(@StringValue,N'Ọ','O');
	SET @StringValue = REPLACE(@StringValue,N'Ø','O');
	SET @StringValue = REPLACE(@StringValue,N'Ộ','O');
	SET @StringValue = REPLACE(@StringValue,N'Ổ','O');
	SET @StringValue = REPLACE(@StringValue,N'Ơ','O');
	SET @StringValue = REPLACE(@StringValue,N'Ỗ','O');
	SET @StringValue = REPLACE(@StringValue,N'Ỏ','O');
	SET @StringValue = REPLACE(@StringValue,N'Ỡ','O');
	SET @StringValue = REPLACE(@StringValue,N'Ở','O');
	SET @StringValue = REPLACE(@StringValue,N'Ƥ','P');
	SET @StringValue = REPLACE(@StringValue,N'Ρ','P');
	SET @StringValue = REPLACE(@StringValue,N'Ŗ','R');
	SET @StringValue = REPLACE(@StringValue,N'Ř','R');
	SET @StringValue = REPLACE(@StringValue,N'Ʀ','R');
	SET @StringValue = REPLACE(@StringValue,N'Ŕ','R');
	SET @StringValue = REPLACE(@StringValue,N'ß','S');
	SET @StringValue = REPLACE(@StringValue,N'Š','S');
	SET @StringValue = REPLACE(@StringValue,N'Ś','S');
	SET @StringValue = REPLACE(@StringValue,N'Ƨ','S');
	SET @StringValue = REPLACE(@StringValue,N'Ş','S');
	SET @StringValue = REPLACE(@StringValue,N'Ŝ','S');
	SET @StringValue = REPLACE(@StringValue,N'Þ','TH');
	SET @StringValue = REPLACE(@StringValue,N'Ť','T');
	SET @StringValue = REPLACE(@StringValue,N'Ŧ','T');
	SET @StringValue = REPLACE(@StringValue,N'Ţ','T');
	SET @StringValue = REPLACE(@StringValue,N'Ƭ','T');
	SET @StringValue = REPLACE(@StringValue,N'Ʈ','T');
	SET @StringValue = REPLACE(@StringValue,N'Ŭ','U');
	SET @StringValue = REPLACE(@StringValue,N'Ự','U');
	SET @StringValue = REPLACE(@StringValue,N'Ū','U');
	SET @StringValue = REPLACE(@StringValue,N'Ǖ','U');
	SET @StringValue = REPLACE(@StringValue,N'Ụ','U');
	SET @StringValue = REPLACE(@StringValue,N'Ǔ','U');
	SET @StringValue = REPLACE(@StringValue,N'Ù','U');
	SET @StringValue = REPLACE(@StringValue,N'Ů','U');
	SET @StringValue = REPLACE(@StringValue,N'Ǚ','U');
	SET @StringValue = REPLACE(@StringValue,N'Ǜ','U');
	SET @StringValue = REPLACE(@StringValue,N'Ú','U');
	SET @StringValue = REPLACE(@StringValue,N'Ư','U');
	SET @StringValue = REPLACE(@StringValue,N'Û','U');
	SET @StringValue = REPLACE(@StringValue,N'Ü','U');
	SET @StringValue = REPLACE(@StringValue,N'Ũ','U');
	SET @StringValue = REPLACE(@StringValue,N'Ű','U');
	SET @StringValue = REPLACE(@StringValue,N'Ủ','U');
	SET @StringValue = REPLACE(@StringValue,N'Ừ','U');
	SET @StringValue = REPLACE(@StringValue,N'Ữ','U');
	SET @StringValue = REPLACE(@StringValue,N'Ử','U');
	SET @StringValue = REPLACE(@StringValue,N'Ǘ','U');
	SET @StringValue = REPLACE(@StringValue,N'Ứ','U');
	SET @StringValue = REPLACE(@StringValue,N'Ų','U');
	SET @StringValue = REPLACE(@StringValue,N'Ʋ','V');
	SET @StringValue = REPLACE(@StringValue,N'Ŵ','W');
	SET @StringValue = REPLACE(@StringValue,N'Ƴ','Y');
	SET @StringValue = REPLACE(@StringValue,N'Ŷ','Y');
	SET @StringValue = REPLACE(@StringValue,N'Ÿ','Y');
	SET @StringValue = REPLACE(@StringValue,N'Ý','Y');
	SET @StringValue = REPLACE(@StringValue,N'Ỳ','Y');
	SET @StringValue = REPLACE(@StringValue,N'Ỹ','Y');
	SET @StringValue = REPLACE(@StringValue,N'Ỷ','Y');
	SET @StringValue = REPLACE(@StringValue,N'Ỵ','Y');
	SET @StringValue = REPLACE(@StringValue,N'Ž','Z');
	SET @StringValue = REPLACE(@StringValue,N'Ź','Z');
	SET @StringValue = REPLACE(@StringValue,N'Ż','Z');
	SET @StringValue = REPLACE(@StringValue,N'Ƶ','Z');
	
	--Lower Case
	SET @StringValue = REPLACE(@StringValue,N'ẩ','a');
	SET @StringValue = REPLACE(@StringValue,N'ẳ','a');
	SET @StringValue = REPLACE(@StringValue,N'ẫ','a');
	SET @StringValue = REPLACE(@StringValue,N'ẵ','a');
	SET @StringValue = REPLACE(@StringValue,N'ậ','a');
	SET @StringValue = REPLACE(@StringValue,N'ặ','a');
	SET @StringValue = REPLACE(@StringValue,N'ǟ','a');
	SET @StringValue = REPLACE(@StringValue,N'ǎ','a');
	SET @StringValue = REPLACE(@StringValue,N'ă','a');
	SET @StringValue = REPLACE(@StringValue,N'ấ','a');
	SET @StringValue = REPLACE(@StringValue,N'ª','a');
	SET @StringValue = REPLACE(@StringValue,N'ả','a');
	SET @StringValue = REPLACE(@StringValue,N'ằ','a');
	SET @StringValue = REPLACE(@StringValue,N'ą','a');
	SET @StringValue = REPLACE(@StringValue,N'à','a');
	SET @StringValue = REPLACE(@StringValue,N'á','a');
	SET @StringValue = REPLACE(@StringValue,N'â','a');
	SET @StringValue = REPLACE(@StringValue,N'ã','a');
	SET @StringValue = REPLACE(@StringValue,N'ầ','a');
	SET @StringValue = REPLACE(@StringValue,N'ä','a');
	SET @StringValue = REPLACE(@StringValue,N'å','a');
	SET @StringValue = REPLACE(@StringValue,N'æ','ae');
	SET @StringValue = REPLACE(@StringValue,N'ā','a');
	SET @StringValue = REPLACE(@StringValue,N'μ','a');
	SET @StringValue = REPLACE(@StringValue,N'ắ','a');
	SET @StringValue = REPLACE(@StringValue,N'ạ','a');
	SET @StringValue = REPLACE(@StringValue,N'ƃ','b');
	SET @StringValue = REPLACE(@StringValue,N'ƀ','b');
	SET @StringValue = REPLACE(@StringValue,N'ƅ','b');
	SET @StringValue = REPLACE(@StringValue,N'ċ','c');
	SET @StringValue = REPLACE(@StringValue,N'ç','c');
	SET @StringValue = REPLACE(@StringValue,N'ƈ','c');
	SET @StringValue = REPLACE(@StringValue,N'č','c');
	SET @StringValue = REPLACE(@StringValue,N'ć','c');
	SET @StringValue = REPLACE(@StringValue,N'ç','c');
	SET @StringValue = REPLACE(@StringValue,N'ĉ','c');
	SET @StringValue = REPLACE(@StringValue,N'¢','c');--maybe special character (currency)
	SET @StringValue = REPLACE(@StringValue,N'đ','d');--maybe z not d
	SET @StringValue = REPLACE(@StringValue,N'ð','d');
	SET @StringValue = REPLACE(@StringValue,N'₫','d');
	SET @StringValue = REPLACE(@StringValue,N'ď','d');
	SET @StringValue = REPLACE(@StringValue,N'ƌ','d');
	SET @StringValue = REPLACE(@StringValue,N'è','e');
	SET @StringValue = REPLACE(@StringValue,N'Ə','e');
	SET @StringValue = REPLACE(@StringValue,N'ĕ','e');
	SET @StringValue = REPLACE(@StringValue,N'é','e');
	SET @StringValue = REPLACE(@StringValue,N'ê','e');
	SET @StringValue = REPLACE(@StringValue,N'ế','e');
	SET @StringValue = REPLACE(@StringValue,N'ể','e');
	SET @StringValue = REPLACE(@StringValue,N'ë','e');
	SET @StringValue = REPLACE(@StringValue,N'ə','e');
	SET @StringValue = REPLACE(@StringValue,N'ė','e');
	SET @StringValue = REPLACE(@StringValue,N'ę','e');
	SET @StringValue = REPLACE(@StringValue,N'ě','e');
	SET @StringValue = REPLACE(@StringValue,N'ệ','e');
	SET @StringValue = REPLACE(@StringValue,N'ẹ','e');
	SET @StringValue = REPLACE(@StringValue,N'ẻ','e');
	SET @StringValue = REPLACE(@StringValue,N'ẽ','e');
	SET @StringValue = REPLACE(@StringValue,N'ǝ','e');
	SET @StringValue = REPLACE(@StringValue,N'ề','e');
	SET @StringValue = REPLACE(@StringValue,N'ē','e');
	SET @StringValue = REPLACE(@StringValue,N'ễ','e');
	SET @StringValue = REPLACE(@StringValue,N'£','e');--maybe special character (currency)
	SET @StringValue = REPLACE(@StringValue,N'ſ','f');
	SET @StringValue = REPLACE(@StringValue,N'ƒ','f');
	SET @StringValue = REPLACE(@StringValue,N'ĝ','g');
	SET @StringValue = REPLACE(@StringValue,N'ğ','g');
	SET @StringValue = REPLACE(@StringValue,N'ġ','g');
	SET @StringValue = REPLACE(@StringValue,N'ǥ','g');
	SET @StringValue = REPLACE(@StringValue,N'ǧ','g');
	SET @StringValue = REPLACE(@StringValue,N'ģ','g');
	SET @StringValue = REPLACE(@StringValue,N'ƣ','g');
	SET @StringValue = REPLACE(@StringValue,N'ĥ','h');
	SET @StringValue = REPLACE(@StringValue,N'ħ','h');
	SET @StringValue = REPLACE(@StringValue,N'ƕ','h');
	SET @StringValue = REPLACE(@StringValue,N'ḥ','h');
	SET @StringValue = REPLACE(@StringValue,N'ĭ','i');
	SET @StringValue = REPLACE(@StringValue,N'ì','i');
	SET @StringValue = REPLACE(@StringValue,N'í','i');
	SET @StringValue = REPLACE(@StringValue,N'ị','i');
	SET @StringValue = REPLACE(@StringValue,N'î','i');
	SET @StringValue = REPLACE(@StringValue,N'ï','i');
	SET @StringValue = REPLACE(@StringValue,N'ī','i');
	SET @StringValue = REPLACE(@StringValue,N'ǐ','i');
	SET @StringValue = REPLACE(@StringValue,N'ı','i');
	SET @StringValue = REPLACE(@StringValue,N'ĩ','i');
	SET @StringValue = REPLACE(@StringValue,N'į','i');
	SET @StringValue = REPLACE(@StringValue,N'ỉ','i');
	SET @StringValue = REPLACE(@StringValue,N'ĳ','ij');
	SET @StringValue = REPLACE(@StringValue,N'ĵ','j');
	SET @StringValue = REPLACE(@StringValue,N'ķ','k');
	SET @StringValue = REPLACE(@StringValue,N'ĸ','k');
	SET @StringValue = REPLACE(@StringValue,N'ƙ','k');
	SET @StringValue = REPLACE(@StringValue,N'ǩ','k');
	SET @StringValue = REPLACE(@StringValue,N'ł','l');
	SET @StringValue = REPLACE(@StringValue,N'ƚ','l');
	SET @StringValue = REPLACE(@StringValue,N'ĺ','l');
	SET @StringValue = REPLACE(@StringValue,N'ļ','l');
	SET @StringValue = REPLACE(@StringValue,N'ľ','l');
	SET @StringValue = REPLACE(@StringValue,N'ŀ','l');
	SET @StringValue = REPLACE(@StringValue,N'µ','m');--maybe special character (currency)
	SET @StringValue = REPLACE(@StringValue,N'Ɯ','m');--maybe w (reserved m)
	SET @StringValue = REPLACE(@StringValue,N'ñ','n');
	SET @StringValue = REPLACE(@StringValue,N'ň','n');
	SET @StringValue = REPLACE(@StringValue,N'ń','n');
	SET @StringValue = REPLACE(@StringValue,N'ŉ','n');
	SET @StringValue = REPLACE(@StringValue,N'ƞ','n');
	SET @StringValue = REPLACE(@StringValue,N'ņ','n');
	SET @StringValue = REPLACE(@StringValue,N'ŋ','n');
	SET @StringValue = REPLACE(@StringValue,N'ò','o');
	SET @StringValue = REPLACE(@StringValue,N'ó','o');
	SET @StringValue = REPLACE(@StringValue,N'ố','o');
	SET @StringValue = REPLACE(@StringValue,N'ô','o');
	SET @StringValue = REPLACE(@StringValue,N'õ','o');
	SET @StringValue = REPLACE(@StringValue,N'ö','o');
	SET @StringValue = REPLACE(@StringValue,N'ø','o');
	SET @StringValue = REPLACE(@StringValue,N'ő','o');
	SET @StringValue = REPLACE(@StringValue,N'ō','o');
	SET @StringValue = REPLACE(@StringValue,N'ớ','o');
	SET @StringValue = REPLACE(@StringValue,N'ŏ','o');
	SET @StringValue = REPLACE(@StringValue,N'ộ','o');
	SET @StringValue = REPLACE(@StringValue,N'ồ','o');
	SET @StringValue = REPLACE(@StringValue,N'ọ','o');
	SET @StringValue = REPLACE(@StringValue,N'ơ','o');
	SET @StringValue = REPLACE(@StringValue,N'ơ','o');
	SET @StringValue = REPLACE(@StringValue,N'œ','oe');
	SET @StringValue = REPLACE(@StringValue,N'ờ','o');
	SET @StringValue = REPLACE(@StringValue,N'ǒ','o');
	SET @StringValue = REPLACE(@StringValue,N'ổ','o');
	SET @StringValue = REPLACE(@StringValue,N'ợ','o');
	SET @StringValue = REPLACE(@StringValue,N'ỏ','o');
	SET @StringValue = REPLACE(@StringValue,N'ỗ','o');
	SET @StringValue = REPLACE(@StringValue,N'ở','o');
	SET @StringValue = REPLACE(@StringValue,N'ỡ','o');
	SET @StringValue = REPLACE(@StringValue,N'¤','o');--maybe special character
	SET @StringValue = REPLACE(@StringValue,N'ƥ','p');
	SET @StringValue = REPLACE(@StringValue,N'ρ','p');
	SET @StringValue = REPLACE(@StringValue,N'ŕ','r');
	SET @StringValue = REPLACE(@StringValue,N'ŗ','r');
	SET @StringValue = REPLACE(@StringValue,N'ř','r');
	SET @StringValue = REPLACE(@StringValue,N'ŝ','s');
	SET @StringValue = REPLACE(@StringValue,N'ƨ','s');
	SET @StringValue = REPLACE(@StringValue,N'š','s');
	SET @StringValue = REPLACE(@StringValue,N'ş','s');
	SET @StringValue = REPLACE(@StringValue,N'ś','s');
	SET @StringValue = REPLACE(@StringValue,N'$','s');
	SET @StringValue = REPLACE(@StringValue,N'þ','th');
	SET @StringValue = REPLACE(@StringValue,N'ť','t');
	SET @StringValue = REPLACE(@StringValue,N'ŧ','t');
	SET @StringValue = REPLACE(@StringValue,N'ţ','t');
	SET @StringValue = REPLACE(@StringValue,N'ƭ','t');
	SET @StringValue = REPLACE(@StringValue,N'ü','u');
	SET @StringValue = REPLACE(@StringValue,N'ù','u');
	SET @StringValue = REPLACE(@StringValue,N'ú','u');
	SET @StringValue = REPLACE(@StringValue,N'û','u');
	SET @StringValue = REPLACE(@StringValue,N'ů','u');
	SET @StringValue = REPLACE(@StringValue,N'ụ','u');
	SET @StringValue = REPLACE(@StringValue,N'ǜ','u');
	SET @StringValue = REPLACE(@StringValue,N'ǔ','u');
	SET @StringValue = REPLACE(@StringValue,N'ū','u');
	SET @StringValue = REPLACE(@StringValue,N'ǘ','u');
	SET @StringValue = REPLACE(@StringValue,N'ủ','u'); 
	SET @StringValue = REPLACE(@StringValue,N'ử','u');
	SET @StringValue = REPLACE(@StringValue,N'ừ','u');
	SET @StringValue = REPLACE(@StringValue,N'ữ','u');
	SET @StringValue = REPLACE(@StringValue,N'ǖ','u');
	SET @StringValue = REPLACE(@StringValue,N'ứ','u');
	SET @StringValue = REPLACE(@StringValue,N'ų','u');
	SET @StringValue = REPLACE(@StringValue,N'ŭ','u');
	SET @StringValue = REPLACE(@StringValue,N'ự','u');
	SET @StringValue = REPLACE(@StringValue,N'ũ','u');
	SET @StringValue = REPLACE(@StringValue,N'ǚ','u');
	SET @StringValue = REPLACE(@StringValue,N'ư','u');
	SET @StringValue = REPLACE(@StringValue,N'ű','u');
	SET @StringValue = REPLACE(@StringValue,N'ŵ','w');
	SET @StringValue = REPLACE(@StringValue,N'ƴ','y');
	SET @StringValue = REPLACE(@StringValue,N'ŷ','y');
	SET @StringValue = REPLACE(@StringValue,N'ý','y');
	SET @StringValue = REPLACE(@StringValue,N'ÿ','y');
	SET @StringValue = REPLACE(@StringValue,N'ỳ','y');
	SET @StringValue = REPLACE(@StringValue,N'ỹ','y');
	SET @StringValue = REPLACE(@StringValue,N'ỷ','y');
	SET @StringValue = REPLACE(@StringValue,N'ỵ','y');
	SET @StringValue = REPLACE(@StringValue,N'¥','y');--maybe special character (currency)
	SET @StringValue = REPLACE(@StringValue,N'×','x');--maybe pecial character (multiplication)
	SET @StringValue = REPLACE(@StringValue,N'ž','z');
	SET @StringValue = REPLACE(@StringValue,N'ź','z');
	SET @StringValue = REPLACE(@StringValue,N'ż','z');
	SET @StringValue = REPLACE(@StringValue,N'ƶ','z');

	--Specials
	SET @StringValue = REPLACE(@StringValue,N'#','-');
	SET @StringValue = REPLACE(@StringValue,N'\','');
	SET @StringValue = REPLACE(@StringValue,N'/','-');
	SET @StringValue = REPLACE(@StringValue,N':','-');
	SET @StringValue = REPLACE(@StringValue,N';','-');
	SET @StringValue = REPLACE(@StringValue,N'*','');
	SET @StringValue = REPLACE(@StringValue,N'?','');
	SET @StringValue = REPLACE(@StringValue,N'"','');
	SET @StringValue = REPLACE(@StringValue,N'<','');
	SET @StringValue = REPLACE(@StringValue,N'>','');
	SET @StringValue = REPLACE(@StringValue,N'|','-');
	SET @StringValue = REPLACE(@StringValue,N'&','-');
	SET @StringValue = REPLACE(@StringValue,N'%','');
	SET @StringValue = REPLACE(@StringValue,N'.','');
	SET @StringValue = REPLACE(@StringValue,N'''','');
	SET @StringValue = REPLACE(@StringValue,N'#','');
	SET @StringValue = REPLACE(@StringValue,N'[','');
	SET @StringValue = REPLACE(@StringValue,N']','');
	SET @StringValue = REPLACE(@StringValue,N'+','-');
	SET @StringValue = REPLACE(@StringValue,N'„','-');
	SET @StringValue = REPLACE(@StringValue,N'“','-');
	SET @StringValue = REPLACE(@StringValue,N' ','-');
	SET @StringValue = REPLACE(@StringValue,N'®','');
	SET @StringValue = REPLACE(@StringValue,N'°','');
	SET @StringValue = REPLACE(@StringValue,N'©','');
	SET @StringValue = REPLACE(@StringValue,N'(','');
	SET @StringValue = REPLACE(@StringValue,N')','');
	SET @StringValue = REPLACE(@StringValue,N'!','');
	SET @StringValue = REPLACE(@StringValue,N'¡','');
	SET @StringValue = REPLACE(@StringValue,N',','-');
	SET @StringValue = REPLACE(@StringValue,N'=','-');
	SET @StringValue = REPLACE(@StringValue,N'_','-');
	SET @StringValue = REPLACE(@StringValue,N'`','');
	SET @StringValue = REPLACE(@StringValue,N'{','');
	SET @StringValue = REPLACE(@StringValue,N'}','');
	SET @StringValue = REPLACE(@StringValue,N'~','');
	SET @StringValue = REPLACE(@StringValue,N'§','');
	SET @StringValue = REPLACE(@StringValue,N'¦','');
	SET @StringValue = REPLACE(@StringValue,N'¨','');
	SET @StringValue = REPLACE(@StringValue,N'«','');
	SET @StringValue = REPLACE(@StringValue,N'»','');
	SET @StringValue = REPLACE(@StringValue,N'¬','');
	SET @StringValue = REPLACE(@StringValue,N'®','');
	SET @StringValue = REPLACE(@StringValue,N'¯','');
	SET @StringValue = REPLACE(@StringValue,N'°','');
	SET @StringValue = REPLACE(@StringValue,N'±','-');
	SET @StringValue = REPLACE(@StringValue,N'´','');
	SET @StringValue = REPLACE(@StringValue,N'¶','');
	SET @StringValue = REPLACE(@StringValue,N'·','');
	SET @StringValue = REPLACE(@StringValue,N'¸','');
	SET @StringValue = REPLACE(@StringValue,N'÷','');
	SET @StringValue = REPLACE(@StringValue,N'ǃ','');

	SET @StringValue = LOWER(@StringValue);

	RETURN  @StringValue;
END
