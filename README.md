# Landing Page - Студия разработки ПО

Современный лендинг для студии разработки программного обеспечения на русском языке. Построен на Vite + React + TypeScript + Tailwind CSS.

## Демо

![Preview](https://cdn.poehali.dev/templates/landing-page/preview.png)

## Особенности

- Полностью на русском языке
- Адаптивный дизайн (mobile-first)
- Анимации с Framer Motion и GSAP
- Интерактивная сетка изображений с эффектом параллакса
- Современный UI с использованием shadcn/ui компонентов
- Оптимизирован для SEO

## Технологии

- **React 18** - UI библиотека
- **Vite** - сборщик
- **TypeScript** - типизация
- **Tailwind CSS** - стилизация
- **Framer Motion** - анимации
- **GSAP** - продвинутые анимации
- **Radix UI** - доступные компоненты
- **Lucide React** - иконки

## Быстрый старт

```bash
# Установка зависимостей
npm install

# Запуск dev-сервера
npm run dev

# Сборка для продакшена
npm run build

# Предпросмотр сборки
npm run preview
```

## Структура проекта

```
src/
├── components/
│   ├── ui/                    # UI компоненты (shadcn/ui)
│   │   └── grid-motion.tsx    # Анимированная сетка
│   └── SoftwareDevelopmentWebsite.tsx  # Главный компонент
├── pages/
│   ├── Index.tsx              # Главная страница
│   └── NotFound.tsx           # 404 страница
├── lib/
│   └── utils.ts               # Утилиты
├── hooks/                     # Кастомные хуки
├── index.css                  # Глобальные стили
├── App.tsx                    # Корневой компонент
└── main.tsx                   # Точка входа
```

## Настройка

### Бренд

Отредактируйте компонент `Logo` в файле `src/components/SoftwareDevelopmentWebsite.tsx`:

```tsx
const Logo = ({ className }: { className?: string }) => {
  return (
    <div className={cn("flex items-center space-x-2", className)}>
      <div className="bg-orange-500 rounded-lg p-2">
        <Code className="h-6 w-6 text-white" />
      </div>
      <span className="text-xl font-bold">ВашБренд</span>
    </div>
  )
}
```

### Контактные данные

Обновите контактную информацию в секции footer:

- Email: `info@kodmaster.ru`
- Телефон: `+7 (495) 123-45-67`
- Адрес: `ул. Технопарковая, 15, Москва`

### Изображения

Изображения для сетки находятся в массиве `gridItems`. Замените URL на свои:

```tsx
const gridItems = [
  "https://your-cdn.com/image1.jpg",
  "https://your-cdn.com/image2.jpg",
  // ...
]
```

## Лицензия

MIT
