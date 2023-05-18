erDiagram
  Salesperson ||--o{ Car : sells
  Customer ||--o{ Car : buys
  Salesperson ||--o{ Invoice : generates
  Customer ||--o{ Invoice : receives
  Car ||--o| CarService : has
  Mechanic }|--|| Car : works on
  Car ||--o{ ServiceTicket : has
  Salesperson {
    string Salesperson_ID
    string Name
    string ContactInformation
    ...
  }
  Customer {
    string Customer_ID
    string Name
    string ContactInformation
    ...
  }
  Car {
    string Car_ID
    string Model
    string Manufacturer
    numeric Price
    ...
  }
  Invoice {
    string Invoice_ID
    date Date
    numeric TotalAmount
    ...
  }
  CarService {
    string Service_ID
    string ServiceDescription
    ...
  }
  Mechanic {
    string Mechanic_ID
    string Name
    string Specialization
    ...
  }
  ServiceTicket {
    string Ticket_ID
    date Date
    ...
  }
