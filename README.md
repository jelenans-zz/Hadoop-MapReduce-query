Hadoop-MapReduce-query
======================

Given the input author-book tuples, map-reduce program procudes a JSON object which contains all the books from only the queried author in a JSON array


The program uses a combiner to minimize number of key-value pairs generated from each node.


Query is given in the following format:

***********************************************

hadoop jar queryauthor.jar org.hwone.QueryAuthor <input> <output> <author>

************************************************

Example output for one author:

{"author":"J. K. Rowling","books":"[{"book":"Harry Potter a vězeň z Azkabanu"},{"book":"Harry Potter and the Goblet of Fire"},{"book":"Garri Potter i filosofskiĭ kamenʹ"},{"book":"Harry Potter i l'orde del fènix"},{"book":"Harry Potter 2 und die Kammer des Schreckens. Meine Freunde. Ausgabe Illustration"},{"book":"Harry Potter und der Orden des Phónix"},{"book":"Garri Potter i kubok ognya"},{"book":"Harri Potter Maen Yr Athronydd"},{"book":"Harry Potter und der Stein der Weisen.  Bd. 1.  9 CDs"},{"book":"Harrī Poṭṭur aur pāras pathar"},{"book":"Harry Potter and the Half-Blood Prince"},{"book":"Harry Potter and the Order of the Phoenix"},{"book":"Hali Bote yu mi shi"},{"book":"Hari Poṭer ṿe-even ha-ḥakhamim"},{"book":"Harry Potter i więzień Azkabanu"},{"book":"Harry Potter and the Half-Blood Prince"},{"book":"Hari Patter va Sang-i Jādū"},{"book":"Harry Potter y La Camara Secreta (Harry Potter and the Chamber of Secrets)"},{"book":"Una vacante imprevista"},{"book":"Garri Potter i taĭnai︠a︡ komnata"},{"book":"Harry Potter & chirec croc lyua"},{"book":"[Areios Poter kai he tou philosophos lithos]"},{"book":"Harry Potter i komnata tajemnic"},{"book":"Harry Potter und der Orden des Phónix"},{"book":"Harri Potter i filosofsʹkyĭ kaminʹ"},{"book":"Harry Potter a L'ecole Des Sorciers / Harry Potter and the Sorcerer's Stone (Harry Potter (French))"},{"book":"Harry Potter & the Order Phoenix/Coming (Harry Potter)"},{"book":"Hǣri Phō̜ttœ̄ kap hō̜nghǣng khāmlap"}]"}
