# Tugas-Web-Service-1

DTD adalah Document Type Definition. DTD mendefinisikan struktur elemen dan atribut dari dokumen XML. DTD digunakan untuk memverifikasi bahwa data XML valid.

Contoh DTD :
Jadwal TV DTD

<!DOCTYPE TVSCHEDULE [ //untuk mengidentifikasi jenis dokumen HTML

<!ELEMENT TVSCHEDULE (CHANNEL+)>
<!ELEMENT CHANNEL (BANNER,DAY+)>
<!ELEMENT BANNER (#PCDATA)>
<!ELEMENT DAY (DATE,(HOLIDAY|PROGRAMSLOT+)+)>
<!ELEMENT HOLIDAY (#PCDATA)>
<!ELEMENT DATE (#PCDATA)>
<!ELEMENT PROGRAMSLOT (TIME,TITLE,DESCRIPTION?)>
<!ELEMENT TIME (#PCDATA)>
<!ELEMENT TITLE (#PCDATA)> 
<!ELEMENT DESCRIPTION (#PCDATA)>

//<!ELEMENT == mendefinisikan bahwa elemen pesan mengandung beberapa elemen

<!ATTLIST TVSCHEDULE NAME CDATA #REQUIRED>
<!ATTLIST CHANNEL CHAN CDATA #REQUIRED>
<!ATTLIST PROGRAMSLOT VTR CDATA #IMPLIED>
<!ATTLIST TITLE RATING CDATA #IMPLIED>
<!ATTLIST TITLE LANGUAGE CDATA #IMPLIED>

//<!ATTLIST == teks yang tidak membentuk markup
]>
