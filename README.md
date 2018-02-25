# Шаблон для compilers (QBE)
Это небольшой Makefile для C-проектов, который должен упростить работу с написанием программ под QBE.


## Сборка QBE
```
git submodule update --init --recursuve
make qbe
```


## Использование
Исходный код программ пишется прямо в корне репозитория. Необходимое условие для успешной сборки -- исходники должны оканчиваться на .c

## Компиляция
```
make
# или с указанием build-директории
make BUILD_DIR=build/
# по-умолчанию BUILD_DIR - корень репозитория
```

После компиляции, бинари разложатся в директории `BUILD_DIR/bin/`

## Дерево скомпилированного проекта
```
.
├── 2gk.c
├── 2rd.c
├── bin
│   ├── 2gk
│   └── 2rd
├── directories
├── include
│   └── qbe -> /home/ochaton/study/comilers/hw/qbe
├── Makefile
├── obj
│   ├── 2gk.o
│   └── 2rd.o
├── qbe
├── README.md
└── tests
```