# IComponent
Func decodeURIComponent($sURIComponent)     If StringRegExp($sURIComponent, "%[0-9A-Fa-f]{2}", 0) Then         $sURIComponent = Execute('"' &amp; StringRegExpReplace($sURIComponent,"(%)([0-9A-Fa-f]{2})",'" &amp; Chr(Dec(''$2'')) &amp; "') &amp; '"')     EndIf     Return $sURIComponent EndFunc   ;==>decodeURIComponen
