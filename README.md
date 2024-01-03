# Система, оснавана на знания, реализирана с Пролог

## 1.	Същност на решаваната задача
Експертната системата идентифицира дадено умствено заболяване или увреждане, използвайки правила и факти.
Идентификацията се осъществява чрез задаване на въпроси, на които потребителя може да отговоря с „да“ или „не“  или там, където се изисква, се дава пълен отговор 
като е дадено меню от възможни отговори.

## 2.	Структура и съдържание на решаваната задача
 


Експертната система индетифицира умствени заболявания(mental disorders). Възможните умствени заболявания са 10, които са класифицирани в 4 типа:
•	Eating disorder
•	Neurodevelopmental disorder
•	Psychotic disorder
•	Genetic disorder

Тип Eating disorder, отговаря на критериите
-	психика(mentality): силно желание да бъдеш слаб (strong desire to be thin)
-	симптом(symptom): абнормални(неправилни) хранителни навици (abnormal eating habits)

Тип Neurodevelopmental disorder, отговаря на критериите
-	състояние(condition): засегната нервна система (affected nervous system)
-	причина(cause): генетични заложби или влияние на средата (genetic and environmental)
-	функциониране на мозъка(brain function): абнормално (abnormal)

 Тип Psychotic disorder, отговаря на критериите
-	психика(mentality): маниакална и депресивна(manic and depressive)
-	симптом(symptom): вяра в неща,които не са реални (false beliefs) 
-	причина(cause): генетични залобни или влияние на средата(genetic and environmental)

Тип Genetic disorder, отговаря на критериите
-	причина(cause): аномалии в генома(abnormalities in genome)

### MENTAL DISORDERS
- Anorexia nervosa - type(eating disorder), consequence(low weight), food amount(food restriction).
- Bulimia Nervosa - type(eating disorder), consequence(purging), food amount(binge eating).
- Asperger syndrome - type(neurodevelopmental disorder), specialty(psychiatry), social skill(low), behavior(repetitive and restricted).
- Dyslexia - type(neurodevelopmental disorder),  specialty(psychiatry), social skill(low), behavior(repetitive and restricted).
- Autism - type(neurodevelopmental disorder), social skill(low), symptom(impaired communication).
- Tourette’s syndrome - type(neurodevelopmental disorder), social skill(normal), specialty(neurology), symptom(motor tics).
- Bipolar disorder - type(psychotic disorder), indication(elevated moods).
- Schizophrenia - type(psychotic disorder), indication(hallucinations).
- Down syndrome - type(genetic disorder), symptom(delayed physical growth), Face features(long and narrow), ears features(large), brain function(intellectual disability).
- Fragile X syndrome - type(genetic disorder), face features(small chin and slanted eyes), brain function(intellectual disability).

## 3.	Стратегията на работа на интерпретатора на знания – обяснение на работата на Пролог в използвания вариант.
  Използван е вграденият в Пролог - backward chaining. Това е техниката за извод, която използва IF-THEN правила, като разбива многократно целта на подцели.
Интерпретаторът доказва или опровергава всяка цел.
Правилата са използвани за представяне на знания, а интерпретатора на пролог за достигане на заключения. 
Пример:\
IF\
&nbsp; &nbsp; &nbsp; type is neurodevelopmental disorder\
&nbsp; &nbsp; &nbsp; and the symptom is impaired communication\
&nbsp; &nbsp; &nbsp; and the skill level is low\
THEN\
&nbsp; &nbsp; &nbsp; the mental disorder is Autism

## 4.Видът на получения резултат 
Целта на системата е да се избере най-добрия избор от много възможности.
Като резултата след достигане на крайната цел ще изведе “Condition was diagnosed as ….”
и достиганатото умствено заболяване и ще завърши с true.
Ако не успее да достигне до такова ще завърши с "The diagnose was not found"

------------------------------------------------------------------------------------------------------------------------------------------------------------------


# Knowledge-based system implemented with Prolog

## 1.	Nature of the problem to be solved
The expert system identifies a mental illness or disability using rules and facts.
Identification is done by asking questions to which the user can answer yes or no or, where required, a complete answer is given 
by giving a menu of possible answers.

## 2.	Structure and content of the problem to be solved
 


The expert system identifies mental disorders. There are 10 possible mental disorders which are classified into 4 types:
- Eating disorder
- Neurodevelopmental disorder
- Psychotic disorder
- Genetic disorder

Eating disorder type meets the criteria
- psyche(mentality): strong desire to be thin
- symptom: abnormal eating habits

Neurodevelopmental disorder type, meets criteria
- condition: affected nervous system
- cause: genetic or environmental influences
- brain function: abnormal

 Type Psychotic disorder, meets criteria
- mentality: manic and depressive
- symptom: belief in things that are not real (false beliefs) 
- cause: genetic or environmental influences

Genetic disorder type, meets criteria
- cause: abnormalities in genome

### MENTAL DISORDERS
- Anorexia nervosa - type(eating disorder), consequence(low weight), food amount(food restriction).
- Bulimia Nervosa - type(eating disorder), consequence(purging), food amount(binge eating).
- Asperger syndrome - type(neurodevelopmental disorder), specialty(psychiatry), social skill(low), behaviour(repetitive and restricted).
- Dyslexia - type(neurodevelopmental disorder), specialty(psychiatry), social skill(low), behaviour(repetitive and restricted).
- Autism - type(neurodevelopmental disorder), social skill(low), symptom(impaired communication).
- Tourette's syndrome - type(neurodevelopmental disorder), social skill(normal), specialty(neurology), symptom(motor tics).
- Bipolar disorder - type(psychotic disorder), indication(elevated moods).
- Schizophrenia - type(psychotic disorder), indication(hallucinations).
- Down syndrome - type(genetic disorder), symptom(delayed physical growth), Face features(long and narrow), ears features(large), brain function(intellectual disability).
- Fragile X syndrome - type(genetic disorder), face features(small chin and slanted eyes), brain function(intellectual disability).

## 3.	The strategy of knowledge interpreter - explanation of Prolog work in the used variant.
  Backward chaining was used as built in Prolog. This is an inference technique that uses IF-THEN rules by repeatedly breaking the target into subgoals.
The interpreter proves or disproves each goal.
The rules are used to represent knowledge and the Prolog interpreter to reach conclusions. 
Example.
IF\
&nbsp; &nbsp; &nbsp; type is neurodevelopmental disorder\
&nbsp; &nbsp; &nbsp; and the symptom is impaired communication\
&nbsp; &nbsp; &nbsp; and the skill level is low\
THEN
&nbsp; &nbsp; &nbsp; the mental disorder is Autism

## 4.The type of result obtained 
The goal of the system is to select the best choice from many possibilities.
As the result after reaching the final goal will output "Condition was diagnosed as ...."
and the mental illness reached and will end with true.
If it fails to reach one it will end with "The diagnosis was not found"

Translated with www.DeepL.com/Translator (free version)
