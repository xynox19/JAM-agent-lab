GOALS:

&nbsp;   ACHIEVE check\_numbers;



PLAN: {



GOAL:

&nbsp;   ACHIEVE check\_numbers;

BODY:



&nbsp;   ASSIGN $N 1;



&nbsp;   WHILE: TEST (<= $N 10)

&nbsp;   {

&nbsp;       WHEN: TEST (= (% $N 2) 0)

&nbsp;       {

&nbsp;           EXECUTE println "N is even";

&nbsp;       }

&nbsp;       WHEN: TEST (!= (% $N 2) 0)

&nbsp;       {

&nbsp;           EXECUTE println "N is odd";

&nbsp;       }



&nbsp;       EXECUTE println "number is " $N;

&nbsp;       ASSIGN $N (+ $N 1);

&nbsp;   };



FAILURE:

&nbsp;   EXECUTE println "program failed";

}



