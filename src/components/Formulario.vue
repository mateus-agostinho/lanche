<template>
  <form action="#" method="POST" class="form">
    <h3 class="form-title">Cadastrar Produto</h3>
    <div class="grid-2">
      <div class="form-controll">
        <div class="form-input">
          <input type="text" name="first_name" required />
          <label for="first_name">Nome</label>
        </div>
      </div>
      <div class="form-controll">
        <div class="form-input">
          <input type="text" name="last_name" id="last_name" required />
          <label for="last_name">Preço</label>
        </div>
      </div>
    </div>
    <div class="form-controll">
      <div class="form-input">
        <input type="email" name="email" id="email" required />
        <label for="email">Descrição</label>
      </div>
    </div>

    <div class="grid-2">
      <div class="form-controll">
        <div class="form-input">
          <input type="password" name="password" id="password" required />
          <label for="password">Categoria</label>
          <div class="password-showHide"></div>
        </div>
      </div>
      <div class="form-controll">
      </div>
    </div>
    <div class="form-submit">
      <button type="submit">Cadastrar</button>
    </div>
  </form>
</template>

<script>

export default{
  name: 'For',
}

</script>

<style scoped>
  .form-title {
    color: #00c5b2;
    font-size: 22px;
    font-weight: 500;
    text-transform: uppercase;
    text-align: center;
    margin: 15px 0px 50px 0px;
}

.form {
    position: relative;
    width: 100%;
    max-width: 550px;
    padding: 15px 30px;
    background: white;
    box-shadow: 0px 0px 3px rgb(208 208 208 / 30%);
    border-radius: 4px;
}

.form-controll {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
}

.form-controll:not(:last-of-type) {
    margin-bottom: 33px;
}

.form-input {
    position: relative;
    width:100%;
}

.form-input input,
.form-input textarea {
    position: relative;
    width:100%;
    padding: 8px 23px 8px 0px;
    outline: 1px solid transparent;
    border: 1px solid transparent;
    border-bottom: 1px solid #c2c2c2;
    background: transparent !important;
    z-index: 9;
    color: #2c3638;
}

.form-controll label  {
    position: absolute;
    left: 0px;
    bottom: 10px;
    color: #c2c2c2;
    font-size: 14px;
    z-index: 1;
    transition: all 0.1s ease-in;
}

input:focus + label {
    opacity: 1;
    bottom: 100%;
    z-index: 9;
    transition: all 0.1s ease-in-out;
}

input:focus {
    border-bottom: 1px solid #00c5b2;
}

/* while input input is not empty */
input:valid + label {
    bottom: 100%;
    z-index: 9;
    transition: all 0.1s ease-in-out;
}

.form-submit {
    position: relative;
    width:100%;
    margin: 14px 0px;
}

.form-submit button {
    width:100%;
    padding: 8px;
    background: #00c5b191;
    font-weight: 500;
    font-size: 14px;
    border-radius: 4px;
    display: flex;
    align-items: center;
    justify-content: center;
    border: 1px solid transparent;
    text-transform: uppercase;
    transition: all 0.2s ease;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    letter-spacing: 0.5px;
    color: #FFF;
    cursor: pointer;
}

.form-submit button:hover {
    background: #00c5b2;
    transition: all 0.2s ease-out;
}

.grid-2 {
    position: relative;
    width:100%;
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-gap: 30px;
}

.password-showHide{
    position: absolute;
    right: 0px;
    top: 50%;
    display: grid;
    transform: translateY(-50%);
    cursor: pointer;
    z-index:99;
}

.password-showHide .icon {
    grid-row: 1/2;
    grid-column: 1/2;
}

.password-showHide .icon path {
    fill: #c2c2c2;
    transition: all 0.2s ease;
}

.password-showHide:hover .icon path {
    fill: #2c3638;
    transition: all 0.2s ease;
}

.password-showHide .icon.show-password {
    opacity: 1;
    z-index: 9;
}
.password-showHide .icon.hide-password {
    opacity: 0;
    z-index: -1;
}

.password-showHide.hide .icon.show-password {
    opacity: 0;
    z-index: -1;
}

.password-showHide.hide .icon.hide-password {
    z-index: 9;
    opacity: 1;
}
</style>