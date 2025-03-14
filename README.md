# Oasis

## Что это

Проект вдохновлен "Оазисом" из фильма "Первому игроку приготовиться".

Данный проект включает в себя несколько под-проектов:

1. `CAPI`
    **Console API** - *API* для простого взаимодействия с консолью
    
    Включает в себя:
    - кросс-плафторменную поддержку графического цветоного вывода в консоль (TUI)
    - поддержку и обработку HID (получение позиции мыши в терминале), получение нажатой клавиши

2. `GTTP`
    **Game Text Transfer Protocol** - протокол, разработанный для сетевой связи клиентов (для онлайн состовляющей игры)

3. `PySandbox`
    **Python Sandbox** - система для изолированного запуска *python* скриптов для осуществления скриптинга игр

## Что сделано сейчас

Сейчас сделан протокол и сервер для него на C++ и Python, а также сделан клиент игры на Python, однако там имеются странные баги, поэтому было решено переписать его на C++, переписав *CAPI* на C++

### Ray tracing

Сделана базовая трассировка лучей для 3D. Протестировано на X11, для компиляции:

```
./tools/cmp --file=raytracing.cpp --only-run=true!
```

Для запуска:

```
./tools/cmp --file=raytracing.cpp --only-run=true
```