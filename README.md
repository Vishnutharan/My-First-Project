# My_Projects

A collection of early academic projects: a C# WinForms hall booking application ("Yarl Hall Booking"), a PHP hall booking website with a login system, Java data-structure exercises for a flight booking system, and design/archive files.

## Contents

| Path | What it is | Tech |
| --- | --- | --- |
| `Final_Ad/` | **C# Hall_Managment**: Visual Studio solution `Final_Ad.sln` with a Windows Forms app for hall booking. It has login, admin and staff forms, customer registration (`newcustomer`), bookings, a booking list and a booking view. | C#, .NET Framework 4.5, WinForms, SQL Server LocalDB |
| `Hall Booking/Login_System/` | A PHP hall booking website with registration and login, admin and user pages, and booking create/edit/delete/view pages under `Home/Final Ass/`. | PHP, MySQL (`mysqli`), HTML, CSS |
| `Flight Booking System DSA/` | Java source saved as `.txt` files: a flight booking program (`ABC_Flyt_Booking`), binary search, linear search, queue and stack exercises. | Java |
| `Fonterra.xd` | An Adobe XD design file | Adobe XD |
| `Cooling Glass Website.zip` | A zip archive of a website project | — |

## Folder structure

```text
My-First-Project/
├── Final_Ad/
│   ├── Final_Ad/
│   └── Final_Ad.sln
├── Flight Booking System DSA/
├── Hall Booking/
│   └── Login_System/
├── .editorconfig
├── .gitignore
├── Cooling Glass Website.zip
├── Fonterra.xd
└── README.md
```

## Running the projects

### C# WinForms app (`Final_Ad/`)

Prerequisites: Windows, Visual Studio with .NET desktop development, .NET Framework 4.5 targeting pack, and SQL Server Express LocalDB.

1. Open `Final_Ad/Final_Ad.sln` in Visual Studio.
2. The connection strings in the forms are hard-coded to `Data Source=(LocalDB)\v11.0` with `AttachDbFilename` pointing to a `HallBookingManagement.mdf` file in the original author's `Documents` folder. Change them to point at your own database. The database file and schema are not in this repository.
3. Build and run (F5). The app starts with `Form2`.

### PHP website (`Hall Booking/Login_System/`)

Prerequisites: PHP with the `mysqli` extension and MySQL/MariaDB, for example via XAMPP or WAMP.

1. Copy the `Login_System` folder into your web server's document root (e.g. `htdocs`).
2. Create a MySQL database named `system_login` with the tables the pages use. No SQL schema is included.
3. Set the database host, user and password in `config.php` and `Home/Final Ass/db_action/db_connection.php`. The defaults are a local `root` user.
4. Open `http://localhost/Login_System/login_form.php` in a browser.

### Java DSA exercises (`Flight Booking System DSA/`)

The files are Java classes saved with a `.txt` extension, each with a `package` declaration. To run one, copy it into a Java project (or rename it to `<ClassName>.java` inside a folder matching its package) and compile it with a JDK.

## Notes

- Visual Studio build output (`bin/`, `obj/`) and user files (`*.suo`) are no longer tracked. They are listed in `.gitignore`.
