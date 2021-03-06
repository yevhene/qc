# Інструменти для роботи з квантовими комп'ютерами
Для роботи з квантовим комп'ютерам можна використовувати реальний квантового комп'ютеру або симулювати його роботу.

## Cпособи задавання квантового алгоритму
1. QASM - спеціальна мова подібна до асемлерної [1];
2. Схема - створення схеми в графічному режимі;
3. Предметно-орієнтована мова (Domain-specific language) - інструменти для симуляції розповсюджуються у вигляді бібліотеки для певної мови програмування та надають програмний інтерфейс.

## Симуляція
Є велика кількість розробок для симуляції роботи квантового комп’ютера. Велика кількість розробок більше не підтримується [2].

### Перелік актуальних розробок

#### Локальні симулятори
Симуляція відбувається на комп'ютері користувача. Від потужності комп'ютера залежить кількість кубітів що можуть опрацьовуватись одночасно.

#### LIQUi|⟩
Симулятор розроблений Microsoft. Високо оптимізование використання па'мяті, що дозволяє симулювати одночансу роботу до 30 кубіт на локальному комп'ютері. [3]

##### Режими симуляції LIQUi|⟩ [4]
LIQUi|⟩ підтримує три режими симуляції:
1. Фізичне моделювання - симуляція що намагається відтворити фізичні аспекти роботи квантового комп'ютера. Симуляція повільна у зв'язку з тим, що доводиться вирішувати велику кількість диферинційних рівнянь. Може оперувати відносно невеликою кількістю кубітів (до 30);
2. Універсальне моделювання - гнучка симуляція що може оперувати з великою кількістю різних операцій (враховуючи ті що задав користувач). Може оперувати невеликою кількістю кубітів (до 30);
3. Стабілізаційне моделювання - може опрацьовувати велику кількість кубітів одночасно (~10000). Обмежене невеликою кількістю операцій що можуть виконуватись (група Кліфорда [5]).

#### Онлайн симулятори
Симуляція відбувається онлайн, зазвичай в хмарному середовищі.

- Forest - дозволяє симулювати роботу 26-кубітового квантового комп'ютера. Доступ через програмний інтерфейс (Python). [6]
- IBM Q Experience - надає доступ до симуляції на 5-ти кубітовому комп'ютеру через графічний інтерфейс, та до 16-ти і 20-ти кубітовому комп'ютеру через програмний інтерфейс QISKIT (Python). [7]
- QuantumPlayground - симулятор квантового комп'ютера від Google. Графічній інтерфейс та 22-кубіта. [8]

## Доступ до реального квантового комп'ютері
Наразі є декілька квантових ком'ютерів що надають доступ онлайн.

- Forest - надає доступ до реального 19-кубітового квантового комп'ютера. Доступ через програмний інтерфейс (Python). Безкоштовно. [6]
- IBM Q Experience - дозволяє працювати на 5-ти кубітовому комп'ютеру через графічний інтерфейс, та до 16-ти і 20-ти кубітовому комп'ютеру через програмний інтерфейс QISKIT (Python). 5-ти та 16-ти кубітові процесори - безкоштовно. 20-ти кубітові процесор тільки для партнерів. [7]
- Quantum in the Cloud - розроблений The University of Bristol. Надає безкоштовний доступ до квантового комп'ютера на 4 кубіта. [9]

## Список джерел
1. Andrew W. Cross, Lev S. Bishop, John A. Smolin, Jay M. Gambetta. Open Quantum Assembly Language. https://arxiv.org/abs/1707.03429
2. List of QC simulators. https://www.quantiki.org/wiki/list-qc-simulators
3. LIQUi|⟩ by Microsoft. http://stationq.github.io/Liquid/
4. LIQUi|⟩ User’s Manual. https://msr-quarc.github.io/Liquid/LIQUiD.pdf
5. Maris Ozols. Clifford group. http://home.lu.lv/~sd20008/papers/essays/Clifford%20group%20[paper].pdf
6. Forest. https://www.rigetti.com/index.php/forest
7. IBM Q Experience. https://www.research.ibm.com/ibm-q/
8. QuantumPlayground by Google. http://www.quantumplayground.net
9. Quantum in the Cloud by The University of Bristol http://www.bristol.ac.uk/physics/research/quantum/engagement/qcloud/
