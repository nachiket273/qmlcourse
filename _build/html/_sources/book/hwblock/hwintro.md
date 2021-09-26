(hwintro)=

# О блоке

Этот блок включает в себя обзор различных подходов к физической реализации квантовых вычислений. Как и классические
компьютеры, квантовые компьютеры вовсе не обязаны быть основаны на какой-то одном физическом принципе работы: информация
может храниться в токах и напряжениях в электрической схеме, спинах атомов, механическом положении или движении
микроскопических частиц. Квантовая механика проявляется для любых достаточно малых систем. В качестве критерия малости
можно использовать постоянную Планка $\hbar$, которая имеет размерность фазового объема, или произведения координаты на
импульс; это отражается и в принципе неопределенность Гейзенберга. Это значит, что если мы имеем систему, работающей на
частоте $\omega$, разность энергий уровней, в которых хранится информация, скорее всего будет порядка $\hbar \omega$.
Из-за того, что $\hbar\sim 1.054\times 10^{-34}~\mathrm{J}\cdot\mathrm{s}$ -- очень маленькое число, два квантовых
состояния очень слабо отличаются друг от друга.

# Обзор и классификация физических платформ для квантовых вычислений

## Радиочастотные и оптические кубиты

На сегодняшнем этапе все платформы для квантовых вычислений можно разделить на два класса: те, которые работают со сравнительно
низкими $\omega/2\pi\sim10^{5}\dots10^{10}~\mathrm{Hz}$ частотами (вплоть до микроволновых), и те, которые работают на
высоких частотах $\omega/2\pi\sim10^{13}\dots10^{15}~\mathrm{Hz}$. К первым относятся

- Сверхпроводниковые квантовые схемы,
- Кубиты на тонком и сверхтонком расщеплении в нейтральных атомах,
- Кубиты на сверхтонком расщеплении в ионах,
- Кубиты спинах в квантовых точках,
- Кубиты на экзотических квазичастицах, вроде Майорановских фермионов.

К второй группе относятся

- Оптические и телекоммуникационные фотонах,
- Кубиты на оптических переходах в атомах и ионах.

Квантовые компьютеры первого типа надо сильно охлаждать, так как они самовозбуждаются под действием броуновского движения и теплового
излучения тел, находящихся при комнатной температуре.

## Природа степени свободы для кодирования информации

Можно классифицировать популярные платформы для квантовых
вычислений и по другим признакам. Например, есть кубиты на естественных степенях свободы и кубиты на коллективных
степенях свободы. Естественные степени свободы -- это

- Любые переходы в уединенных атомах и ионах,
- Фотоны в открытом пространстве.

Кубиты на естественных степенях свободы автоматически получаются одинаковыми: вы берете одинаковые атомы, и у них
обязательно будут одинаковые переходы. Впрочем, если поместить их в какую-нибудь ловушку, то из-за того, что ловушки
немного влияют на частоты переходов в атомах, эту эквивалентность легко испортить. Кубиты на искусственных степенях
свободы получаются когда имеет место коллективная динамика большого числа частиц, например поляризация в материала
оптоволокна, или коллективное движение электронов в сверхпроводнике. Примеры искусственных степеней свободы:

- Сверхпроводниковые электрические цепи,
- Фотоны в интегрально-оптической схеме,
- Фотоны в оптоволокне,
- Спины в квантовых точках,
- Любые квазичастицы в твердотельных системах.

На самом деле граница между естественными степенями свободы и искусственными вовсе не такая очевидная, как может
показаться на первый взгляд. Так, например, фотон, находящийся в открытом пространстве, можно поместить между двумя
зеркалами, которые образуют резонатор. Но в таком случае в зеркалах, и в носителях заряда в зеркале будет храниться
часть энергии фотона -- получается так называемый "поляритон", который уже не совсем естественная степень свободы.
Абсолютно тождественными могут быть только те носители информации, которые ни с чем не связаны.

## Способ кодирования информации

Только системы, где есть всего два уровня, а больше никакие не используются и не учитываются, строго говоря являются
кубитами. Такими являются, например

- Потоковые сверхпроводниковые кубиты,
- Логические кубиты, которые получаются выполнением кодов коррекции на большом числе физических кубитов любой природы;

Помимо "чистых" кубитов, у которых есть всего два дискретных состояния, существуют также "кудиты", которые имеют
$d$ ($d>2$) состояний. Таковыми являются, например:

- Ионы со сложной структурой уровней и правилами отбора переходов между ними,
- Сверхпроводниковые кубиты-трансмоны,
- Атомы и ридберговские состояния в них.

Бывают модели квантовых вычислений на непрерывных степенях свободы, например:

- Оптические вычисления на непрерывных переменных,
- Колебательное движение ионов в радиочастотных ловушках,
- Состояния микроволнового поля в сверхпроводниковых резонаторах.

## Способ выполнения операций

Модели вычислений в квантовы компьютерах можно классифицировать по признаку способа реализации операций в них.
Самый простой и очевидный способ -- воздействие на кубит (кудит, напрерывную переменную) при помощи короткого
аналогового сигнала на резонансной частоте этой системы, причем амплитуда и фаза этого сигнала будет определять
унитарную матрицу операции. Так работают

- Сверхпроводниковые кубиты-трансмоны и потоковые кубиты,
- Кубиты на ионах в радиочастотных ловушках
- Кубиты на нейтральных атомах в дипольных ловушках.

Бывают вычислительные модели, в которых вместо временной последовательности управляющих сигналов носитель информации
движется по "конвееру", вдоль которого с ним выполняются операции. Так работают, например, вычисления на

- фотонах в интегральной оптике,
- фотонах в открытом пространстве.

Некоторые модели вычислений вовсе не предполагают выполнения каких-то изолированных операций. Впрочем, для таких моделей
вычислений и не выполняется большинство утверждений и теоретических предсказаний, связанных с квантовыми вычислениями.
Таковыми моделями является, например,

- квантовый аннилер D-Wave,

Важно отметить, что классические компьютеры работают совсем иначе, чем все вышеперечисленные квантовые компьютеры. В них
операции осуществляются цифровыми сигналами, то есть от непосредственного значения уровня сигнала слабо зависит то,
какая операция будет выполнена, главное, чтобы сигнал вовремя превысил некоторое пороговое значение. Цифровой характер
классических компьютеров имеет очень важное значение для масштабирования алгоритмов, ведь именно он обеспечивает
воспроизводимость и возможность безошибочной работы квантового компьютера. К моделям квантовых вычислений,
нечувствительным к аналоговым ошибкам управляющих сигналов, или с пониженной чувствительностью к ним, можно отности

- кубиты на майорановских феромионах,
- логические кубиты, которые получаются в результате работы алгоритмов квантовой коррекции ошибок на физических кубитах
любой природы,
- сверхпроводниковые 0-пи кубиты, при условии, что гейты будут производиться специальным помехозащищенным образом, а не
через промежуточные уровни.

## Наборы инструкций и универсальность

Разные модели вычислений дают разные наборы инструкций для реализации квантовых алгоритмов. В зависимости от вероятности
успешной реализации инструкций (квантовые компьютеы делают ошибки!) эти модели вычислений могут быть ближе, либо дальше
от создания универсального масштабируемого квантового компьютера. По этому признаку

- сверхпроводниковые кубиты,
- нейтральные атомы,
- ионы в радиочастотных ловушках

являются самыми очевидными. Набор инструкций в них содержит однокубитные и двухкубитные операции, инициализацию кубита в
определенном состоянии и считывание. Чем выше точность операций -- тем лучше, и все операции на сегодняшний день
продемонстированы в вероятностью положительного исхода выше 99% -- этого все еще мало для многих применений, но это уже
что-то.

Для вычислений на линейнооптических схемах используются источники единичных эквивалентных фотонов, либо источники запутанных
фотонов, либо источники сжатого света. Вероятность успеха операции по созданию такого излучения (либо степень сжатия
света) на сегодняшний день сильно далека от того, что нужно для универсальности квантовых вычислений; здесь идет речь о
сжатии порядка 10 дБ (грубо переводя на язык "успешного выполнения операции" 0,9), и вероятности испускания фотона 0,9.
Однако отсутствие универсальности не означает, что линейнооптические схемы должны быть для всех задач вычислительно
слабее, чем другие платформы: напротив, самое сильное квантовое превосходство на сагодняшний день достигнуто именно на
таких устройствах.

Причина, по которой линейнооптические системы выделяются среди других заключается в том, что для полноценного компьютера
(что классического, что квантового) нужны нелинейные элементы. В классическом компьютере  это транзисторы. На одних
линейных индуктивностях и емкостях можно, в зависимости от способа кодирования информации, выполнять какой-то набор
операций, но универсальным он не будет, потому что функция отклика линейной цепи является линейным. Алгоритмы, которые
не сводятся к умножению матрицы на вектор в некотором представлении данных, на линейной системе выполнитель не получится.
Чтобы обойти это ограничение, линейно-оптические системы для квантовых вычислений принимают на часть своих входов, в
дополнение к входным данным, сложные неклассические сигналы, а на выходе производится считывание числа фотонов, которое
является квадратичнм по отношению к амплитудам сигналов. Дополнение линейной оптики наборами нелинейых операций
может сделать такие модели вычислений универсальными.

Наконец, кубиты с дискретными операциями, такие как логические кубиты и кубиты на майорановских фермионах, сами по себе
не дают полный набор квантовых логических операций -- в дополнение к ним нужны обычные кубиты. Впрочем, задача пстроения
кубита на майоранвским фермионах, либо на коррекции ошибок сама по себе настолько сложная, что необходимость связать с
ним обыкновенные дополнительные кубиты не кажется такой сложной.

## Успехи в практической реализации

Наконец, платформы для квантовых вычислений можно отсортировать по максимальному размеру гильбертового пространства и
точности операций (не только унитарных гейтов, но и считыванию и инициализации), которое удавалось реализовать
экспериментально. В этом рейтинге только три верхние платформы находятся относительно
близко к режиму квантового превосходства в подтвержденных экспериментальных работах. Итак, рейтинг:

- Линейная оптика (фотоны) в открытом пространстве,
- Сверхпроводниковые кубиты-трансмоны,
- Ионы в линейных радиочастотных ловушках,
- Интегральнооптические фотоны,
- Нейтральные атомы в дипольных ловушках,
- Спины в квантовых точках.

Другие платформы существуют на сегодняшний день в лучшем случае в виде двухкубитной системы, чаще в виде одного
кубита, а лучше вообще в виде теоретической концепции -- которая может оказаться вовсе нереализуемой на практике.

## Заключение

Из-за того, что все платформы для квантовых вычислений очень разные, делать конкретные утверждения про все сразу
практически невозможно. Вместо этого мы будем рассматривать один типа платформ -- сверхпроводниковые кубиты.