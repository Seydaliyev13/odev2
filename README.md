 # odev2
 #adressden query kısmının alınması parse yolu
#from urllib.parse import urlparse, parse_qs
#url ="http://www.example.org/default.html?adi=can&soyadi=aydın&yas=35&il=izmir"
#x=urlparse(url)
#print(x)
#query1=urlparse(url).query
#print("QUERY_STRİNG1",query1)
#dict1=dict(pair.split("=") for pair in query1.split("&"))

 #adressden query kısmının alınması split yolu
#page,query2=url.split('?')
#print("QUERY_STRİNG2:",query2)
#dict2 = dict(pair.split('=')for pair in query2.split('&'))

degisken="QUERY_STRING='adi=can&soyadi=aydın&yas=35&il=izmir'"
x=degisken[13:]
print(x)
xYeni=x.replace("'","")
sozluk=dict(pair.split("=") for pair in xYeni.split("&"))
print(sozluk)
