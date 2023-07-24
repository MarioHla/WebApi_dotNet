# WebApi_dotNet
Creating Web Api project in .net  
  
2 modela:  
  &nbsp;&nbsp; Locations  (id, name, latitude, longitude, category)  
  &nbsp;&nbsp; Records    (id, RequestTime, RequestUrl, RequestBody, ResponseBody)  
  
Stranica prikazuje 4 endpointa:  
  searchLocationsInRaidus  
      - ulaz: latituda, longituda  
      - izlaz: sve lokacije unutar 100 metara (ako nema lokacija vraća se "Not Found" i pretraga se ne bilježi u tablici "Records")  
  searchByCategory  
      - ulaz: unijeti neku kategoriju  
      - izlaz: sve lokacije kojima "ulaz" == "Location.category"  
  searchByName  
      - ulaz: unijeti neki "name"  
      - izlaz: "Location.category" sadrži "ulaz"  
  printRecords  
      - bilježe se zapisi request i response za svaki puta kada se napravi searchLocationsInRadius (ova metoda ispisuje te zapise)
