## 109、110
- 建立hoc資料夾(higher order component)
- 建立(Aux.js)utility auxiliary componen (此元件會回傳子元件內容)
- 建立 Layout


畫面的組成：1個Layout(外誆)他可以控制位置(ex:padding、margan)裡面有會動的元件(component)用外誆包裝起來。

### 111 Adding a Dynamic Ingredient Component
新增 Burger 資料夾，底下在建立 BurgerIngredient 資料夾

- Burger(Burger.js)
  - BurgerIngredient(BurgerIngredient.js、BurgerIngredient.css)

製作 BurgerIngredient.js 裡面有 switch 多個控制 css (bread-top、salad、becan、cheese)，利用prop

### 112 Adding Prop Type Validation
在 BurgerIngredient.js 中使用 prop-types 參數驗證
```bash
npm install --save prop-types
```
改成 class 寫法並使用 prop-types 的驗證方法。

```js
BurgerIngredient.PropTypes={
  type: PropTypes.string.isRequired
}
```

### 113 Starting the Burger Component
在 Burger.js 元件中 引入 BurgerIngredient 相對應區塊(上麵包、培根、沙拉、肉、下麵包)，完成 Burger 元件。

```js
<div className={classes.Burger}>
      <BurgerIngredient type="bread-top" />
      <BurgerIngredient type="cheese" />
      <BurgerIngredient type="meat" />
      <BurgerIngredient type="bread-bottom" />
</div>
```
已經建立好 Burger 元件後就在(container)BurgerBuilder 容器中引入 Burger 元件。

```js
<Burger/>
```

### 114、115、118 Outputting Burger Ingredients Dynamically

BurgerBuilder 傳遞 state 參數 Burger 的 props 接收得知沙拉、起司、培根要幾個使用動態物件走訪map渲染出來


### 119 Adding the Build Control Component


