# VBA
## bỏ dấu tiếng việt
VBA code
Function bo_dau_tieng_viet(Text As String) As String
  Dim AsciiDict As Object
  Set AsciiDict = CreateObject("scripting.dictionary")
  AsciiDict(192) = "A"
  AsciiDict(193) = "A"
  AsciiDict(194) = "A"
  AsciiDict(195) = "A"
  AsciiDict(196) = "A"
  AsciiDict(197) = "A"
  AsciiDict(199) = "C"
  AsciiDict(200) = "E"
  AsciiDict(201) = "E"
  AsciiDict(202) = "E"
  AsciiDict(203) = "E"
  AsciiDict(204) = "I"
  AsciiDict(205) = "I"
  AsciiDict(206) = "I"
  AsciiDict(207) = "I"
  AsciiDict(208) = "D"
  AsciiDict(209) = "N"
  AsciiDict(210) = "O"
  AsciiDict(211) = "O"
  AsciiDict(212) = "O"
  AsciiDict(213) = "O"
  AsciiDict(214) = "O"
  AsciiDict(217) = "U"
  AsciiDict(218) = "U"
  AsciiDict(219) = "U"
  AsciiDict(220) = "U"
  AsciiDict(221) = "Y"
  AsciiDict(224) = "a"
  AsciiDict(225) = "a"
  AsciiDict(226) = "a"
  AsciiDict(227) = "a"
  AsciiDict(228) = "a"
  AsciiDict(229) = "a"
  AsciiDict(231) = "c"
  AsciiDict(232) = "e"
  AsciiDict(233) = "e"
  AsciiDict(234) = "e"
  AsciiDict(235) = "e"
  AsciiDict(236) = "i"
  AsciiDict(237) = "i"
  AsciiDict(238) = "i"
  AsciiDict(239) = "i"
  AsciiDict(240) = "d"
  AsciiDict(241) = "n"
  AsciiDict(242) = "o"
  AsciiDict(243) = "o"
  AsciiDict(244) = "o"
  AsciiDict(245) = "o"
  AsciiDict(246) = "o"
  AsciiDict(249) = "u"
  AsciiDict(250) = "u"
  AsciiDict(251) = "u"
  AsciiDict(252) = "u"
  AsciiDict(253) = "y"
  AsciiDict(255) = "y"
  AsciiDict(352) = "S"
  AsciiDict(353) = "s"
  AsciiDict(376) = "Y"
  AsciiDict(381) = "Z"
  AsciiDict(382) = "z"
  AsciiDict(258) = "A"
  AsciiDict(259) = "a"
  AsciiDict(272) = "D"
  AsciiDict(273) = "d"
  AsciiDict(296) = "I"
  AsciiDict(297) = "i"
  AsciiDict(360) = "U"
  AsciiDict(361) = "u"
  AsciiDict(416) = "O"
  AsciiDict(417) = "o"
  AsciiDict(431) = "U"
  AsciiDict(432) = "u"
  AsciiDict(7840) = "A"
  AsciiDict(7841) = "a"
  AsciiDict(7842) = "A"
  AsciiDict(7843) = "a"
  AsciiDict(7844) = "A"
  AsciiDict(7845) = "a"
  AsciiDict(7846) = "A"
  AsciiDict(7847) = "a"
  AsciiDict(7848) = "A"
  AsciiDict(7849) = "a"
  AsciiDict(7850) = "A"
  AsciiDict(7851) = "a"
  AsciiDict(7852) = "A"
  AsciiDict(7853) = "a"
  AsciiDict(7854) = "A"
  AsciiDict(7855) = "a"
  AsciiDict(7856) = "A"
  AsciiDict(7857) = "a"
  AsciiDict(7858) = "A"
  AsciiDict(7859) = "a"
  AsciiDict(7860) = "A"
  AsciiDict(7861) = "a"
  AsciiDict(7862) = "A"
  AsciiDict(7863) = "a"
  AsciiDict(7864) = "E"
  AsciiDict(7865) = "e"
  AsciiDict(7866) = "E"
  AsciiDict(7867) = "e"
  AsciiDict(7868) = "E"
  AsciiDict(7869) = "e"
  AsciiDict(7870) = "E"
  AsciiDict(7871) = "e"
  AsciiDict(7872) = "E"
  AsciiDict(7873) = "e"
  AsciiDict(7874) = "E"
  AsciiDict(7875) = "e"
  AsciiDict(7876) = "E"
  AsciiDict(7877) = "e"
  AsciiDict(7878) = "E"
  AsciiDict(7879) = "e"
  AsciiDict(7880) = "I"
  AsciiDict(7881) = "i"
  AsciiDict(7882) = "I"
  AsciiDict(7883) = "i"
  AsciiDict(7884) = "O"
  AsciiDict(7885) = "o"
  AsciiDict(7886) = "O"
  AsciiDict(7887) = "o"
  AsciiDict(7888) = "O"
  AsciiDict(7889) = "o"
  AsciiDict(7890) = "O"
  AsciiDict(7891) = "o"
  AsciiDict(7892) = "O"
  AsciiDict(7893) = "o"
  AsciiDict(7894) = "O"
  AsciiDict(7895) = "o"
  AsciiDict(7896) = "O"
  AsciiDict(7897) = "o"
  AsciiDict(7898) = "O"
  AsciiDict(7899) = "o"
  AsciiDict(7900) = "O"
  AsciiDict(7901) = "o"
  AsciiDict(7902) = "O"
  AsciiDict(7903) = "o"
  AsciiDict(7904) = "O"
  AsciiDict(7905) = "o"
  AsciiDict(7906) = "O"
  AsciiDict(7907) = "o"
  AsciiDict(7908) = "U"
  AsciiDict(7909) = "u"
  AsciiDict(7910) = "U"
  AsciiDict(7911) = "u"
  AsciiDict(7912) = "U"
  AsciiDict(7913) = "u"
  AsciiDict(7914) = "U"
  AsciiDict(7915) = "u"
  AsciiDict(7916) = "U"
  AsciiDict(7917) = "u"
  AsciiDict(7918) = "U"
  AsciiDict(7919) = "u"
  AsciiDict(7920) = "U"
  AsciiDict(7921) = "u"
  AsciiDict(7922) = "Y"
  AsciiDict(7923) = "y"
  AsciiDict(7924) = "Y"
  AsciiDict(7925) = "y"
  AsciiDict(7926) = "Y"
  AsciiDict(7927) = "y"
  AsciiDict(7928) = "Y"
  AsciiDict(7929) = "y"
  AsciiDict(8363) = "d"
  Text = Trim(Text)
  If Text = "" Then Exit Function
  Dim Char As String, _
    NormalizedText As String, _
    UnicodeCharCode As Long, _
    i As Long
  'Remove accent marks (diacritics) from text
  For i = 1 To Len(Text)
    Char = Mid(Text, i, 1)
    UnicodeCharCode = AscW(Char)
    If (UnicodeCharCode < 0) Then
      'See http://support.microsoft.com/kb/272138
      UnicodeCharCode = 65536 + UnicodeCharCode
    End If
    If AsciiDict.Exists(UnicodeCharCode) Then
      NormalizedText = NormalizedText & AsciiDict.Item(UnicodeCharCode)
    Else
      NormalizedText = NormalizedText & Char
    End If
  Next
  bo_dau_tieng_viet = NormalizedText
End Function
## Elimilate dấu phẩy thành các hàng 
Sub SplitAll()
    Dim xRg As Range
    Dim xRg1 As Range
    Dim xCell As Range
    Dim I As Long
    Dim xAddress As String
    Dim xUpdate As Boolean
    Dim xRet As Variant
    On Error Resume Next
    xAddress = Application.ActiveWindow.RangeSelection.Address
    Set xRg  = Application.InputBox("Please select a range", "Kutools for Excel", xAddress, , , , , 8)
    Set xRg  = Application.Intersect(xRg, xRg.Worksheet.UsedRange)
    If xRg Is Nothing Then Exit Sub
        If xRg.Columns.Count > 1 Then
            MsgBox "You can't select multiple columns", , "Hoc Excel Online"
            Exit Sub
            End If
            Set xRg1 = Application.InputBox("Split to (single cell):", "Kutools for Excel", , , , , , 8)
            Set xRg1 = xRg1.Range("A1")
            If xRg1 Is Nothing Then Exit Sub
                xUpdate = Application.ScreenUpdating
                Application.ScreenUpdating = False
                For Each xCell In xRg
                    xRet = Split(xCell.Value, ",")
                    xRg1.Worksheet.Range(xRg1.Offset(I, 0), xRg1.Offset(I + UBound(xRet, 1), 0)) = Application.WorksheetFunction.Transpose(xRet)
                    I = I + UBound(xRet, 1) + 1
                Next
                Application.ScreenUpdating = xUpdate
            End Sub
