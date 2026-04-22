# Database schema design of the book my show application

## 1. **Schema's**
### a. List of entities

- **User**
    
    | **user_id** | **name** | **role** | **date_of_birth** |
    |-------------|----------|----------|-------------------|
    | 1           | Akshay   | Admin    | 24-05-1995        |
    | 2           | John     | User     | 01-12-1991        |
    If more business logic with role relies on create separate table for roles as **Role**.


- **Movie**
  
   | **movie_id** | **name** | **genre** | **rating** | **min_age** |
   |--------------|----------|-----------|------------|-------------|
   | 1            | Avatar   | Sci-Fi    | 9.7        | 12          |
   | 2            | KGF      | Violence  | 9.5        | 18          |

- **Theatre**

    | **theatre_id** | **theatre_name** | **capacity** | **screens** | **city** |
    |---------|--------------|------|----|----------|
    | 1 | PVR | 70 | 4  | Delhi    |
    | 2 | Mahalakshmi | 340 | 1  | Bengaluru |

- **Show**

  | **show_id** | **movie_id** | **theatre_id** | **time_slot** |
  |-------------|--------------|----------------|---------------|
   | 1           | 1            | 1              | 10AM          |
  | 2           | 1            | 1              | 12PM          |
  | 4           | 2            | 1              | 09PM          |
  | 5           | 1            | 2              | 09PM          |
  | 6           | 1            | 2              | 10AM          |
  | 6           | 2            | 1              | 04PM          |

- **Seat**

    | **seat_id** | **category** | **price_in_rupees** | 
    |-------------|--------------|---------------------|
    | A1          | 4DX          | 600                 |
    | A2          | 4DX          | 600                 |
    | A5          | 4DX          | 600                 |
    | B1          | 2D           | 200                 |
    | B4          | 2D           | 200                 |
    
    