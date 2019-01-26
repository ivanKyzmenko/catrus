<template>
    <header class="main-header container">
        <div class="main-header__left">
            <div class="main-header__left-mobile">
                <span></span><span></span><span></span>
            </div>
            <div class="main-header__left-logo">
                <img class="desktop" src="../assets/icons/logo.png" alt="">
                <img class="main-header__left-logo__mobile mobile" src="../assets/icons/logo-m.png" alt="">
            </div>
        </div>

        <div class="main-header__center">
            <div class="main-header__center-img">
                <img class="desktop" src="../assets/icons/phone.svg" alt="">
                <img class="mobile" src="../assets/icons/phone-m.svg" alt="">

            </div>

            <div class="main-header__center-data">
                <h5 class="main-header__center-data__title">24/7 - Client Support</h5>
                <div class="main-header__center-data__phone">1-888-829-9060</div>
            </div>

            </div>

        <div class="main-header__right">
            <div class="main-header__right-bell desktop">
                <img src="../assets/icons/bell.svg" alt="">
            </div>

            <div class="main-header__right-account">
                <img src="../assets/icons/account.svg" class="main-header__right-account__avatar-m mobile">

                <div class="main-header__right-account__avatar desktop">SF</div>
                <div class="main-header__right-account__data desktop">
                    <span class="main-header__right-account__data-email">design@katrus.ru</span>
                    <span class="main-header__right-account__data-name">Sergey Fateev</span>
                </div>
            </div>

            <div class="main-header__right-order">
                <img src="../assets/icons/order.svg" alt="">
                <span class="mobile">order</span>
                <div class="main-header__right-order__current desktop">2</div>
                <div class="main-header__right-order__total desktop">
                    Total: <b>$768</b>
                </div>
            </div>
        </div>
    </header>
</template>