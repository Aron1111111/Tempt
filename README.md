# 图书俱乐部 / Книжный клуб

在[原项目](https://github.com/Aron1111111/docs)的活动与报名文档基础上，增加活动描述校验和状态转换。代码使用Python，接口约定保存在OpenAPI中。
На основе [исходного проекта](https://github.com/Aron1111111/docs) добавлены проверка описания встречи и переходы статусов. Код написан на Python, API описан в OpenAPI.

## 运行测试 / Запуск тестов

需要Python 3.10及以上版本，不用安装额外依赖。克隆后切换到要检查的分支，再运行测试。
Нужен Python 3.10 или новее, без дополнительных зависимостей. После клонирования выберите ветку и запустите тесты.

```sh
git clone https://github.com/Aron1111111/Tempt.git
cd Tempt
git switch feature/description-validator
python -B -m unittest discover -s tests -v
git switch feature/status-transitions
python -B -m unittest discover -s tests -v
```

本地结果：描述校验分支9项通过，状态分支4项通过。这里记录的是单元测试结果，尚未进行HTTP接口测试。
Локальные результаты: 9 тестов в ветке описания и 4 в ветке статусов пройдены. Это модульные тесты; HTTP-тесты ещё не проводились.

## 文件 / Файлы

- [业务规则](docs/review-requirements.md) / Правила
- [OpenAPI](api/bookclub.openapi.yaml)
- [描述校验PR说明](pr-descriptions/description-validator.md) / Описание PR проверки текста
- [状态转换PR说明](pr-descriptions/status-transitions.md) / Описание PR статусов

