[аип лр9-10.docx](https://github.com/Zhanel18/Zhanel18/files/7511955/9-10.docx)
[Алибекова ТПО18.docx](https://github.com/Zhanel18/Zhanel18/files/7511957/18.docx)

procedure TForm1.Button1Click(Sender: TObject);
var a:array of integer;
    n,i:integer;
begin
  randomize;
n:=SpinEdit1.Value;
Setlength(a,n);
StringGrid1.ColCount:=n;
StringGrid1.RowCount:=1;
StringGrid1.ColCount:=n;
StringGrid1.RowCount:=1;
for i:=0 to n-1 do
   begin
  a[i]:=random(50)+1;
  StringGrid1.Cells[i,0]:=IntToStr(a[i]);
 end;
for i:=0 to n-1 do
StringGrid2.Cells[i,0]:=IntToStr(a[n-i-1]);
end;
end

