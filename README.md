# excel

## email format
=AND(ISERROR(FIND(" ",A1)),LEN(A1)-LEN(SUBSTITUTE(A1,"@",""))=1,IFERROR(SEARCH("@",A1)<SEARCH(".",A1,SEARCH("@",A1)),0),NOT(IFERROR(SEARCH("@",A1),0)=1),NOT(IFERROR(SEARCH(".",A1,SEARCH("@",A1))-SEARCH("@",A1),0)=1),LEFT(A1,1)<>".",RIGHT(A1,1)<>".")
