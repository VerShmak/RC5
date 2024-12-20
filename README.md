# Лабораторная работа "RC5"
В ходе даной работы требуется реализовать:  
 - Генерацию секретого ключа
 - Шифрование текста
 - Дешифрование текста

# Описание алгоритма шифрования
RC5 — блочный шифр. Он является частью семейства шифров RC (Rivest Cipher) и предлагает гибкость в выборе параметров, что позволяет адаптировать его к различным требованиям безопасности и производительности. 

RC5-32/12/16 обозначает алгоритм RC5 c 32-битным блоком, 12 раундами шифрования и 16-байтным ключом. Данная комбинация рекомендуется в качестве основного варианта.

Подготовка ключа:
Для начала на вход поступает целове число, с помощью которого генерируется секретный ключ. Ключ представляет из себя специальный набор чисел, который будет использоваться для шифрования.

Для генерирования ключа мы пользуемся процедурой расширения, которая состоит из трёх функций: выравнивания ключа, инициализации массива расширенных ключей, перемешивания массивов ключей.

Исходный текст, который нужно зашифровать, разбивается на небольшие кусочки фиксированного размера. Если последний кусочек меньше нужного размера, его дополняют. Каждый кусочек данных проходит через несколько этапов обработки. На каждом этапе выполняются математические операции, которые смешивают данные и делают их трудными для понимания.
После обработки всех кусочков они объединяются, и получается зашифрованное сообщение.

# Описание алгоритма дешифрования
Чтобы вернуть данные в исходный вид, используется тот же набор чисел, но операции выполняются в обратном порядке.

# Тестовое задание 
Исходный текст:
Налить в подходящую емкость молоко комнатной температуры, вбить туда яйца, добавить соль и сахар. Постепенно подсыпать муку, при этом помешивая, чтобы не получалось комочков. Довести до консистенции нежирной сметаны. Добавить разрыхлитель. На сильно раскаленную сковороду налить немного масла и жарить блины.

Выбранный размер ключа: 5

#  Результат шифрования
f40a9b1ffa46edaca679224041c148f18d063712c559619eb5afd6e9b4aa503fb660eec6d9d09def002201465d17bd969908355276ba6bf909863916a697afcdc5b0be2dcd1ed370bb816ccb3a3a0b3edc2618e43a5093bfb0a7480ba1167012c996defc5fcaac02435699f5e984396ee1893c3217911da424507587ca26bb75471bab9a47d87bb58d4152c3491f9770a621435d426e8de08998afa3a19e9d68d49326f22cd1d6a5ff549d51a50b45a2a4889b7ee691fda6775a1aeae62119ee2a64cd6d20ddea8eb1ab030b1ae60d5886c845b17bd728a983011a7487ca061e6c670dfda29bbdeb1c590b71818b1d3e34a6683bc5a8b7a5dfefe57ecc1c402573348b19e1d1557d042f3589750840eb23bf1b61754ba2e6fc6f55e8964c062a4cef1817965839e1df14b952f47872f2c1e2be26a4e07627f8f2d956109d7693c9920f9bef095d6f9c64d6b44f58124e51fd95d59eab30640ec88732b182fdc6a055da2d025a5b45820bb5b3dcdb807242e2935a4b34a6fbda021f54f3e3afee289bf3155dd730f20ea5c84cc660fb8129e6a9aa05406f4ce1893c3217911da406ac913cba119d137d6988bee3b846d9e1dfcd67b6a3d7c209bd6f9d5c16e361844271b8bf71cd9f1a3494ccc6607c613f365a925374cdb856ed87b3917dbe986cc905d2b0493b0cd4a6ce354980339d36896c5c031c0f41777f2ec05eb74e4f8bbc6a0874ecb6f26e909ee4dbe09d2b2a03ccbe92bae2d4e8d6fd76f134cb28bab4048efd6cf09cebe38ed673971a2195d3bc7542e74660

# Результат дешифрования
Налить в подходящую емкость молоко комнатной температуры, вбить туда яйца, добавить соль и сахар. Постепенно подсыпать муку, при этом помешивая, чтобы не получалось комочков. Довести до консистенции нежирной сметаны. Добавить разрыхлитель. На сильно раскаленную сковороду налить немного масла и жарить блины.


