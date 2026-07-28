# Ассамблея СО/БУ — проБУди СОзнание · Иркутск 2026

Лендинг региональной ассамблеи подкомитетов СО/БУ в Иркутске (14–15 ноября 2026).

## Файлы

- `index.html` — единый HTML-файл со всей страницей (CSS + JS + 3D Three.js).
- `na-logo-ref.png` — референс логотипа N/A (для истории).

## Запуск

Любой статический сервер в корне:

```bash
python -m http.server 8765
```

Затем открыть http://localhost:8765/index.html

## Стек

- Чистый HTML / CSS / JS (без сборки)
- Three.js r160 через importmap
- Lenis (плавный скролл), GSAP ScrollTrigger
- Three.js post-processing: RoomEnvironment + UnrealBloomPass
- Кастомные 3D-буквы N и A (Shape + ExtrudeGeometry) внутри вращающегося кольца
- Canvas-сеть связей между карточками оргкомитета
- Модальное окно с контактами по клику на карточку
