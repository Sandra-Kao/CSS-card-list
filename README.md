# CSS-card-list
Please see codepen:

https://codepen.io/K-SY/pen/NWpRBMz

```css
:root {
    --color-gray-darker  : #787878;
    --gray-darkest       : #323233;
    --vivid-blue-darker  : #006498;
    --vivid-blue-lightest: #daeef9;
  
    --color-white: #ffffff;
    --color-black: #000000;
    --color-black-50: rgba(0,0,0,.5);

    --color-blue-light: #48ace1;
    --color-blue: #008cd6;
    --color-blue-darker: #006498;

    --color-gray-lighter: #e2e2e2;
    --color-gray-light: #d5d5d5;
    --color-gray-base: #c5c5c5;
    --color-gray-darker: #787878;
}

* {
    margin : 0;
    padding: 0;
}

.typography-title {
    font-size: 32px;
    line-height:42px;
    font-weight: bold;
}

/* ignore */
/* ignore */
/* ignore */

.card-list {
    padding: 48px 50px;
}

.card-list__heading {
    width: 100%;
    margin-top: 8px;
    position: relative;
}

.typography-title {
    display: inline-block;
}

.card-list__viewall {
    display: inline-block;
    right: 0;
    bottom: 0;
    position: absolute;
}

.card-list__wrapper {
    margin: 24px auto;
    /*margin-top: 24px;
    margin-bottom: 24px;*/
    display: flex;
}

.card-list__item {
    border-radius: 4px;
    box-shadow: 0 2px 8px 0 var(--color-gray-base);
    background-color: var(--color-white);
    width: calc((100% - 20px * 3 ) / 4);  
    text-decoration: none;
    overflow: hidden;
}

    .card-list__item:not(:last-child) {
        margin-right: 20px;
    }

    .card-list__item:hover {
        text-decoration: none;
    }

.card-list__content {
    padding: 0 20px;
    padding-bottom: 20px;
}

.card-list__img {
    margin-bottom: 8.5px;
    margin-top: 20px;
    margin-left: 20px
}

.card-list__img--full {
    width: 100%;
    margin-top: 0;
    margin-left: 0;
}

.card-list__img--logo {
    height: 80px;
}

.card-list__img--icon {
    width: 80px;
    height: 80px;
    border-radius: 14px;
    border: 1px solid #c8c8c8;
    background-color: #c8c8c8;
}

.card-list__wrapper.img-large .card-list__img {
    width: 140px;
    height: 140px;
}

.card-list__tag {
    font-size: 14px;
    line-height: 1.43;
    text-transform: uppercase;
    color: var(--color-gray-darker);
}

.card-list__title {
    font-size: 20px;
    font-weight: bold;
    line-height: 1.6;
    color: var(--color-black);
}

.card-list__discription {
    font-size: 14px;
    line-height: 1.43;
    color: var(--color-gray-darker);
}
