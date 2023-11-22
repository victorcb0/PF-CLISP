# PF---CLISP

## Laborator 1

1. Transpose and evaluate the following expressions in Lisp:
   a. \( \frac{(25 + 30) \times 15}{2} \)
   b. \( 6 \times 3.1416 \)

2. Determine the integer quotient for the arithmetic mean of the numbers:
   5, 6.7, -23.2, 75, and 100.3

3. Determine the remainder of the division of the numbers:
   a. \( 365 \div 12 \)
   b. \( 13 \div 467 \)

4. Write in Lisp expression form and evaluate the solutions for the following quadratic equation:
   \( 2x^2 + 7x + 5 = 0 \)

5. Determine the rounded-down and rounded-up integer result, then increment and decrement the result for the expression:
   \( \frac{(5 \times 2.25 - 7.13)}{(45 - \frac{25}{5})} \)

6. Evaluate the following Lisp forms:
   a. \( \text{(* (MAX 3 4 5) (MIN 3 4 5))} \)
   b. \( \text{(EXPT (MAX 3 1 4) (MAX 2 7 1))} \)
   c. \( \text{(REM (+ 5 7 13) (- 14 1))} \)

7. Display the result from problem 3 in the form of a message:
   Example: "The remainder of the division of the numbers ... and ... is: ..."

8. Display a message before reading a variable, then read the variable.
   Example: "a =" read value
   
# Laborator 2

1. Scoateţi simbolul D din următoarele expresii folosind CAR si CDR.
(A B C D)
(A (B C) (D E))
(A (B C (D E)))
((A) (B) (C) (D) (E))
( A (B) ((C)) (((D))) ((((E)))))
((((A) B) C) D)
2. Evaluaţi următoarea expresie Lisp, apoi returnaţi lungimea listei rezultat:
(subst ' azi ' maine (reverse ' (frumoasa zi o este maine)))
3. Evaluaţi ȋn ordine şi argumentaţi rezultatul, următoarele expresii :
(setq lista ’(a b c (d e))
(setq M ’max)
(cons M lista)
(cons lista M)
(append (list M) (last (cdr lista)))
(list ' M (cadr lista))
(append ' lista (list M (last lista)))
(list (car lista) (cadr lista) (caddr lista) M)
4. Se considera lista:
((A) (B) (C) (D) (E))
Folosind toate funcțiile de construcție a listelor și cele de acces la elementele unei liste, contruiți următoarea listă:
((((A) (B) (C)) . B) (E D C) D)
Se evalueaza cu nota maxima acea rezolvare care include toate functiile predefinite prezentate.
5. Se considera lista:
l1 : ((((A) (B)) C) (D) (EF G))
Corectati eroarea aparuta in urma evaluarii expresiei:
(append (cadr l1) (car (nth '1 l1)) (last l1))
Argumentati apoi rezultatul evaluarii expresiei:
(cons (nth '3 l1) (nthcdr '2 l1))
6. Evaluând expresiile urmatoare, obţineţi rezultatele:
> (setq E '(x y ((z) u)) F (last E) G (caar F))
(Z)
>(setq X '12 Y '14 Z '22 E (- (+ x y) z))
4
>(setq M (MIN 1 -4 23 56 1) P (* M 10) X (EXPT P 2))
1600
Evaluaţi pentru fiecare expresie ȋn parte simbolurile şi argumentaţi rezultatul.
7. Se considera lista:
(A B C D)
Folosind functia SUBST impreuna cu alte functii, obtineti din lista initiala lista:
(D B C A)
Folosind functia REVERSE impreuna cu alte functii, obtineti din lista initiala, lista:
(D A B C)

# Laborator 3

1. Exprimați cu ajutorul lui if modulul unui număr şi operatorul not:
(abs x) (not y)
2. Exprimați cu ajutorul lui cond : and, or ȋntre 3 argumente:
(or x y z) (and u v w)
3. Determinați cu ajutorul lui cond elementul din mijloc dintre trei elemente numerice.
4. Definiți funcțiile my-third, my-last,care să returneze al trei-lea element al unei liste, respectiv ultimul element al unei liste.
5. Definiți o funcție my-append care primeşte ca argumente doi parametri de tip listă şi returnează o listă de lungime dublă obținută prin concatenarea celor două liste inițiale. Apoi definiți predicatul palindrom care determină dacă lista astfel obținută este sau nu palindrom.
6. Definiți o funcție care primeşte ca parametri coeficienții unei ecuații de gradul 2 şi care dacă delta este pozitiv returnează o listă cu soluțiile ecuației, dacă delta este egal cu 0, returnează soluția unică a ecuației de gradul 2, iar dacă delta este negativ, returnează mesajul “solutii complexe”.
7. Definiți o funcție care primeşte un singur argument x şi returnează valoarea unei funcții definte astfel:

8. Definiți o funcție care primeşte ca argumente un atom şi o listă, şi returnează o listă ȋn care se adaugă la coada listei inițiale atomul, numai ȋn cazul ȋn care atomul nu se regăseşte ȋn listă. In caz contrar, se returnează fragmentul de listă incepând cu elementul găsit.
9. Definiți o funcție care afişează un meniu interactiv, citeşte câte un caracter şi execută o operație conform caracterului citit, iar ȋn cazul ȋn care caracterul nu este nici unul dintre caracterele citite, returnează un mesaj de eroare.
1 – Adunare
2 – Scadere
3 – Inmulțire
4 – Restul ȋmpărțirii
Se considera trei variabile inițializate cu valori citite de la tastatură , primele două reprezintă două numere intregi, iar ultima, numărul corespunzător operației ce va fi executată. Ȋn corpul lui LET se execută operația corespunzătoare caracterului citit pentru cea de-a treia variabilă.
10. Să se implementeze recursiv o funcţie COUNTATOMS care primeşte ca argument o listă ce conţine şi liste imbricate şi returnează numărul total de elemente ale listei.
11. Să se implementeze funcțiile recursive Rot-left şi Rot-right care rotesc la stânga, respectiv la dreapta n elemente ale unei liste. Rotire la stânga ȋnseamnă mutarea primului element al listei la coada listei. Rotire la dreapta ȋnseamnă mutarea ultimului element al listei ȋn fața listei.
12. Scrieţi o funcţie fără _dubluri ( lista ) care returnează lista fără dubluri. Elementele să fie în aceeaşi ordine în lista returnată ca şi în lista iniţială, păstrându se ultima apariţie a elementelor duplicat.
Exemplu: > ( f a r a _d u b l u r i ‟ ( 1 2 2 3 4 5 6 4 4 ) )  ( 1 2 3 5 6 4 )
13. Implementați recursiv predicatul presentp care determină dacă un atom apare oriunde ȋn interiorul unei liste, chiar şi o listă ce conține liste imbricate.
14. Implementați recursiv o funcție care primeşte ca argument un număr ȋntreg şi returnează lista cu cifrele numărului.
15. Implementați iterativ funcția pozpar, care primeşte ca argument o listă şi returnează o listă cu elmentele de pe pozițiile impare ale listei inițiale.
16. Implementați iterativ o funcție, care determină cel mai mare divizor comun a două numere ȋntregi. Evidenţiaţi parametri actuali şi valoarea rezultată a funcţiei apelate, în ordinea apelurilor, respectiv terminărilor funcţiei pentru un exemplu concret.

# Laborator 4

1. Implementaţi o funcţie care adună toate elementele unei liste, aflate pe poziţii pare. Poziţiile se consideră începând cu 0.
2. Implementaţi recursiv reuniunea,intersecţia şi diferenţa dintre 2 mulţimi folosind remove-if-not.
3. Definiţi o funcţie care numără apariţiile unui număr dat într-o listă generalizată, folosind mapcar şi lambda.
4. Definiţi o funcţie care afişează o listă generalizată sub forma precizată pentru exemplul următor:
(a b (c d) (e f g) h) 
( a
b
( c
d )
( e
f
g )
h )
5. Scrieţi o funcție FETCH care primeşte o cheie şi o listă de asociaţii, iar dacă găseşte cheia va returna doar valoarea ei. Dacă nu o găseşte va returna un mesaj corespunzător.
> (fetch 'temperature '((temperature 100) (pressure (120 60)) (pulse 72)))
100
6. Scrieţi o funcţie ce returnează o listă cu toate cheile dintr-o listă de asociere.
7. Presupunând că avem simboluri ce au proprietatea tata. Definiţi procedura bunic ce primeşte un simbol şi returnează bunicul din partea tatălui dacă este cunoscut, alftel nil.
8. Definiţi funcţia recursivă ADAM care primeşte un simbol şi returnează cel mai îndepărtat strămoş pe linie paternă.
9. Definiţi funcţia recursivă STRAMOSI care returnează o listă formată din persoana împreuna cu toţi strămoşii cunoscuţi, mergând pe două proprietatăti: tata şi mama.
10. Definiţi un macro define care defineşte o funcţie având sintaxa:
(define <nume functie> (<param 1> ... <param n>) <corp>)
11. Definiţi un macro dotimes cu sintaxa:
(dotimes (<var> <count> <rezultat> <corp>)
Prima dată se evaluează <count> care trebuie să fie un întreg. Apoi <var> este succesiv legata la întregi de la 0 la valoarea lui <count> minus 1. Corpul este evaluat de fiecare dată, iar <rezultat> este returnat la sfârşit.
12. Scrieţi o funcţie PRINT-ARRAY care afişează o matrice de două dimensiuni primită ca argument. Fiecare rând al matricii va fi afişat pe o linie nouă. Folosiţi ARRAY-DIMENSION pentru a afla domeniul indicilor.
13. Scrieţi câte o funcţie care transformă o matrice reprezentată ca listă de liste, ȋn ambele moduri prezentate, într-o matrice standard LISP. Determinați apoi numărul elementelor pare ale matricii.
14. Definiţi o structură de tip nod cu elementele: rădăcina stga dr;
Implementaţi apoi o funcţie care adaugă un nou nod, după regula: ȋn stânga pentru valorile <= decât rădăcina, sau ȋn dreapta pentru valori mai mari decât rădăcina. Creaƫi un arbore.
