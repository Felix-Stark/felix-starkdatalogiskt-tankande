G-nivå - Split the nota
Split the nota räknar ut hur mycket varje vän ska betala på exempelvis en restaurang när notan kommer. Användaren matar in summan, antal vänner och sedan dricks (som skrivs i decimalform d.v.s 10% blir 0.10). Skisserna nedan är mest för att ge visuell bild av hur det ser ut, ni behöver inte ha med sådant som "byt vy" eller liknande i er pseudokod.

moment 
   - lägg in summa för mat
   - lägg in antal gäster som ska betala
   - lägg på driksen på summa för mat
   - dela totalsumma (mat + dricks) på antal gäster
      - räkna ut
   - visa pris per person


//START SPLIT THE NOTA

FUNCTION named calculateSplit
   OUTPUT Summa
      INPUT sum of food and bevereges
   OUTPUT Antal vänner
      INPUT number of paying guests
   OUTPUT Dricks
      INPUT percentage of tips in decimal
   OUTPUT Räkna button


   CALCULATE
      ADD 1.0 to percentage of tips in decimal
      MULTIPLY sum of food and bevereges with percentage of tips in decimal
      DIVIDE sum of MULTIPLY with number of paying guests
   
     
      IF Dricks is equal to 0
         THEN OUTPUT Don't be a Scrooge!
      IF input field is left empty
         THEN OUTPUT 'You missed something'
      ELSE OUTPUT Varje person ska betala 'sum of CALCULATE'

ENDFUNCTION

CALL FUNCTION named calculateSplit


