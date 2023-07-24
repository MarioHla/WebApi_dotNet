# WebApi_dotNet
Creating Web Api project in .net  
  
2 modela:  
  &nbsp;&nbsp; Locations  (id, name, latitude, longitude, category)  
  &nbsp;&nbsp; Records    (id, RequestTime, RequestUrl, RequestBody, ResponseBody)  
  
Stranica prikazuje 4 endpointa:  
  &nbsp;&nbsp;searchLocationsInRaidus  
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- ulaz: latituda, longituda  
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- izlaz: sve lokacije unutar 100 metara (ako nema lokacija vraća se "Not Found" i pretraga se ne bilježi u tablici "Records")  
  &nbsp;&nbsp;searchByCategory  
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- ulaz: unijeti neku kategoriju  
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- izlaz: sve lokacije kojima "ulaz" == "Location.category"  
  &nbsp;&nbsp;searchByName  
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- ulaz: unijeti neki "name"  
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- izlaz: "Location.category" sadrži "ulaz"  
  &nbsp;&nbsp;printRecords  
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- bilježe se zapisi request i response za svaki puta kada se napravi searchLocationsInRadius (ova metoda ispisuje te zapise)
