# Predescu-Albert-Victor-631
	Descriere Proiect: Sistem de Autentificare și Înregistrare cu PHP și LocalStorage

Acest proiect reprezintă o aplicație web în care utilizatorii pot vizualiza o listă de filme, iar după autentificare, vor putea adăuga filme în wishlist și favorite. Sistemul folosește PHP pentru gestionarea autentificării și înregistrării utilizatorilor, iar localStorage este folosit pentru a salva datele utilizatorului între sesiuni. În plus, am implementat un design simplu și ușor de utilizat pentru a face interacțiunea mai plăcută.

Structura Proiectului
Proiectul are mai multe fișiere principale care îndeplinesc funcții specifice:

index.html - Pagina principală unde sunt afișate filmele. Dacă utilizatorul nu este autentificat, va fi redirecționat la pagina de login.
login.php - Pagina de autentificare unde utilizatorii își pot introduce datele pentru a se loga.
register.php - Pagina de înregistrare unde utilizatorii pot crea un cont nou.
style.css - Fișierul de stilizare care face ca aplicația să arate bine și să fie ușor de folosit.
auth.php - Fișier care conține logica de autentificare și înregistrare.
database.php - Conexiunea la baza de date, unde sunt stocate datele utilizatorilor.
Cum Funcționează
Autentificare și Înregistrare:

Când utilizatorul accesează aplicația, dacă nu este autentificat, va fi trimis la pagina de login.
La login, utilizatorul trebuie să introducă un nume de utilizator și o parolă. Dacă sunt corecte, va fi autentificat și redirecționat către pagina principală.
Dacă nu are un cont, poate accesa pagina de înregistrare, unde va introduce datele necesare pentru a crea un cont nou. După înregistrare, utilizatorul va fi logat automat.
Gestionarea Filmelor:

Pe pagina principală, utilizatorii pot vedea o listă de filme, fiecare având o descriere și un buton pentru a adăuga filmul în wishlist.
Filmele sunt stocate într-o listă, iar atunci când un film este adăugat la wishlist, acest lucru este salvat în sesiunea utilizatorului.
LocalStorage:

După autentificare, informațiile utilizatorului (de exemplu, numele și starea autentificării) sunt salvate în localStorage pentru a fi disponibile chiar și după închiderea browserului. Astfel, utilizatorii nu trebuie să se autentifice de fiecare dată când revin pe site.
Pagina Principală (index.html):

Pe pagina principală sunt afișate filmele într-un design simplu, organizat pe coloane. Fiecare film are un buton care permite utilizatorului să-l adauge în wishlist.
Securitate:

Parolele utilizatorilor sunt criptate folosind algoritmi moderni (de exemplu, bcrypt) pentru a preveni accesul neautorizat la informațiile sensibile.
Pași Importanți de Urmat
Instalarea unui Server Local:

Am folosit XAMPP pentru a configura un server local, care permite rularea fișierelor PHP pe calculatorul personal.
După instalarea XAMPP, serverul Apache și MySQL trebuie pornite pentru a permite aplicației să ruleze corect.
Baza de Date:

Am creat o bază de date simplă cu un tabel users, care conține coloane pentru username, password, și alte informații necesare pentru înregistrare și autentificare.
Testarea Aplicației:

După configurarea serverului local și a bazei de date, utilizatorul poate accesa index.html printr-un browser și începe să interacționeze cu aplicația.
Este important ca fișierele PHP să fie plasate într-un folder accesibil serverului Apache din XAMPP (de exemplu, în folderul htdocs).
Cum Poți Modifica Aplicația
Dacă vrei să îmbunătățești aplicația sau să adaugi noi funcționalități, poți:

Modifica stilul din style.css pentru a face aplicația să arate mai modern sau pentru a o personaliza după preferințele tale.
Adăuga mai multe funcționalități, cum ar fi un sistem de comentarii pentru filme sau opțiuni suplimentare de filtrare a filmelor.
Extinde baza de date pentru a include mai multe informații despre utilizatori sau filme.
