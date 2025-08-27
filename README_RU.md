
Для файла `README_RU.md` (русская версия):
```markdown
[English version](README.md) | [Русская версия](README_RU.md)

# EMForce Simulator: Моделирование электромагнитных взаимодействий

![Визуализация электромагнитного поля](images/field_simulation.png)

## 🚀 О проекте

Инновационная платформа для моделирования электромагнитных взаимодействий, объединяющая:
- Динамическое моделирование сил Лоренца и Ампера
- Интеграцию с ИИ (DeepSeek) для расчетов
- Визуализацию на движке Unity
- Расчет статических полей через FEMM

## ✨ Ключевые особенности

- **Симуляции в реальном времени** электромагнитных явлений
- **ИИ-ассистент** для проектирования электронных схем
- **Глубокая интеграция** между Unity, FEMM и ИИ-компонентами
- **Экспорт** в LTSpice и другие форматы
- **Интерактивная 3D-визуализация** взаимодействия полей

## 🛠 Технологический стек

| Компонент | Технологии |
|-----------|------------|
| Графический интерфейс | Unity, HLSL, URP |
| Физический движок | Кастомный C# движок сил Лоренца |
| Расчет полей | Интеграция с FEMM, Python скрипты |
| ИИ компонент | DeepSeek API, PyTorch |
| Визуализация | Shader Graph, Compute Shaders |

## 📦 Установка

```bash
# Клонирование репозитория
git clone https://github.com/yourusername/emforce-simulator.git
cd emforce-simulator

# Установка зависимостей
pip install -r requirements.txt

# Запуск демо-симуляции
python demo_simulation.py

## 🧪 Пример использования

```python
# Расчет силы Лоренца
def lorentz_force(q, E, v, B):
    """Расчет силы Лоренца"""
    return q * (E + np.cross(v, B))

# Пример параметров
charge = 1.6e-19  # Кл
electric_field = np.array([0, 0, 0])  # В/м
velocity = np.array([1e6, 0, 0])  # м/с
magnetic_field = np.array([0, 0, 1e-3])  # Тл

force = lorentz_force(charge, electric_field, velocity, magnetic_field)
print(f"Сила Лоренца: {force} Н")
```

## 📊 Структура проекта
```
emforce-simulator/
├── src/                 # Исходный код
│   ├── unity/           # Файлы Unity проекта
│   ├── femm/            # Скрипты интеграции с FEMM
│   └── ai/              # Модуль ИИ-ассистента
├── docs/                # Документация
├── simulations/         # Примеры симуляций
├── images/              # Графика и диаграммы
└── README.md            # Этот файл
```

## 🤝 Участие в проекте

Мы приветствуем вклад в следующие области:
- Разработка физических моделей
- Визуализация электромагнитных полей
- Интеграция с дополнительными симуляторами
- Оптимизация алгоритмов

Ознакомьтесь с [руководством по участию](docs/CONTRIBUTING.md) для получения дополнительной информации.

## 📝 Лицензия

Этот проект распространяется под лицензией MIT - подробности см. в файле [LICENSE](LICENSE).

## 📞 Контакты

EN - [rattchanel@gmail.com](mailto:rattchanel@gmail.com)
RU - [tesla2you@mail.ru](mailto:tesla2you@mail.ru)

Ссылка на проект: [https://github.com/IlyaSchastlivchik/emforce-simulator](https://github.com/IlyaSchastlivchik/emforce-simulator)

---

*Разработано с помощью [DeepSeek](https://deepseek.com) и [Unity](https://unity.com)*