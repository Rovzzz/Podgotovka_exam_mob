# Podgotovka_exam_mob
Проект для работы с API

## Начало работы
Для начала работы с приложением вам необходимо скачать и распаковать архив с программой.

## Необходимые условия
* Для запуска программы необходим компьютер на ОС Windows 7 или новее.
>Пакет Net Framework 4.8 или выше.
* Подключение к интернету и БД

# Установка
После распаковки нужно запустить **exe файл**

## Код RetrofitApi
``` java
import retrofit2.Call;
import retrofit2.http.Query;
import retrofit2.http.DELETE;
import retrofit2.http.Body;
import retrofit2.http.POST;
import retrofit2.http.PUT;

public interface RetrofitApi {

    @PUT ("GamesModels")
    Call<Game> updateData (@Query("ID") int id, @Body Game game);

    @POST ("GamesModels")
    Call<Game> postData (@Body Game game);

    @DELETE ("GamesModels")
    Call<Game> deleteData (@Query("ID") int id);
}
```
# Ссылка на репозиторий - [Podgotovka_exam_mob](https://github.com/Rovzzz/Podgotovka_exam_mob)
