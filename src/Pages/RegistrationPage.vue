<template>
    <header>
    <div id="title">
        <h1>Зарегистрируйтесь</h1>
        <select class="change-lang">
            <option value="ru">RU</option>
            <option value="en">EN</option>
            <option value="pl">PL</option>
        </select>
    </div>
    <div id="subtitle">
        <h3>
            <span>или</span>
            <a href="login">войдите в аккаунт</a>
        </h3>
    </div>
</header>
<main>
    <div id="login-form">
        <div class="field">
            <label class="input-label">Выберите клуб</label>
            <select class="input">
                <option value="ru">Двойной Чикаго</option>
                <option value="en">Дворец</option>
            </select>
        </div>
        <div class="field">
            <label class="input-label">Имя</label>
            <input class="input is-error" type="text" placeholder="Введите имя...">
            <p class="error">Обязательно для заполнения</p>
        </div>
        <div class="field">
            <label class="input-label">Фамилия</label>
            <input class="input is-error" type="text" placeholder="Введите фамилию...">
            <p class="error">Обязательно для заполнения</p>
        </div>
        <div class="field">
            <label class="input-label">E-mail</label>
            <input class="input is-error" type="text" placeholder="email@mail.com">
            <p class="error">Обязательно для заполнения</p>
        </div>
        <div class="field">
            <label class="input-label">Пароль</label>
            <input class="input" type="password" placeholder="•••••••••">
            <p class="error">Обязательно для заполнения</p>
        </div>
        <div class="field">
            <label class="input-label">Подтверждение пароля</label>
            <input class="input" type="password" placeholder="•••••••••">
            <p class="error">Обязательно для заполнения</p>
        </div>
        <button type="submit" id="login-button">Зарегистрироваться</button>
    </div>


</main>
</template>

<style scoped>
header {
    display: flex;
    flex-direction: column;
    align-items: center;
}

#title {
    display: flex;
    align-items: center;
}

#subtitle {
    display: flex;
    justify-content: flex-start;
    color: #d1d6d9;
}

    #subtitle a {
        color: #80d4d6;
    }

#title > h1 {
    color: #d1d6d9;
    font-size: 20pt;
}

#title > .change-lang {
    margin: 10px;
    border: 2px solid #80d4d6;
    border-radius: 10px;
    padding: 7px;
    background-color: #151e1d;
    color: #d9dee1;
    cursor: pointer;
    font-weight: bold;
}

#login-form {
    margin-top: 60px;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.input-label {
    color: #bdc7c8;
    font-size: 10pt;
    display: block;
    margin: 5px;
}

.input {
    font-size: 15pt;
    background-color: #0e1316;
    border: 0;
    border-bottom: 3px solid #80d4d6;
    color: #d9dee1;
    padding: 5px;
    width: 100%;
}

    .input::placeholder {
        color: #bdc7c8;
        opacity: 0.25;
    }

.is-error {
    border-bottom: 3px solid orangered;
}

.error {
    color: orangered;
    font-size: 10pt;
    margin: 3px;
}

.input-help {
    display: block;
    font-size: 10pt;
    color: #80d4d6;
}

#login-button {
    color: #80d4d6;
    font-size: 15pt;
    font-weight: bold;
    padding: 10px 30px 10px 30px;
    background-color: #151e1d;
    border: 0;
    border-radius: 20px;
    cursor: pointer;
}

.field {
    margin-bottom: 10px;
    width: 30%
}

@media (max-width: 768px) {
    .field {
        width: 85%;
    }
}
</style>