
# 🎮 Повышение FPS в играх на слабом ПК (без стороннего софта)

Полезный набор твиков, которые реально помогают в играх на слабых системах. Всё вручную, безопасно и без всяких "бустеров".

---

## 🔹 1. Отключение GameBar и DVR

1. Win + I → Игры → **Game Bar** → выключи  
2. В разделе **Захваты** → также всё выключи  
3. В PowerShell от имени администратора:

```powershell
reg add "HKCU\System\GameConfigStore" /v GameDVR_Enabled /t REG_DWORD /d 0 /f
reg add "HKLM\SOFTWARE\Policies\Microsoft\Windows\GameDVR" /v AllowGameDVR /t REG_DWORD /d 0 /f
```

---

## 🔹 2. Отключение визуальных эффектов Windows

1. Win + S → **"Производительность системы"**  
2. Открой → вкладка **Визуальные эффекты**  
3. Включи: **"Обеспечить наилучшее быстродействие"**

Можно вернуть сглаживание шрифтов вручную.

---

## 🔹 3. Отключение фоновых служб

1. Win + R → `msconfig`  
2. Вкладка **Службы** → **Скрыть службы Microsoft**  
3. Отключи ненужные службы (Adobe, Nvidia Telemetry, Discord Update и т.п.)

---

## 🔹 4. Убрать автозагрузку

1. Ctrl + Shift + Esc → **Диспетчер задач**  
2. Вкладка **Автозагрузка**  
3. Отключи всё лишнее (OneDrive, Spotify, Steam Web Helper и т.д.)

---

## 🔹 5. Настройки видеодрайвера

### ▫️ Nvidia:

1. ПКМ по рабочему столу → Панель управления Nvidia  
2. Управление параметрами 3D:  
   - Режим управления питанием: **Предпочтительный режим максимальной производительности**  
   - Ограничение частоты кадров: **Выключить**  
   - Потоковая оптимизация: **Вкл.**

### ▫️ AMD:

1. Radeon Settings → Производительность  
2. Настроить:  
   - Radeon Boost: **Вкл.**  
   - Radeon Chill: **Выкл.**  
   - Повышение производительности — по вкусу

---

## ✅ Результат

- +10–30% FPS на слабых конфигурациях  
- Меньше лагов и фризов  
- Чище фон и быстрая загрузка системы

---

🛠 Автор: @marselcomp
📡 Telegram-канал: @whatmarsel
