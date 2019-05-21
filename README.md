# Módulo de Tabs que funcionam como sliders

* Conteúdo das Tabs estão dentro de Container-Center's
* Adiciona CSS Classes à Tab e ao Container
* Módulo exporta:
  * slider
  * array de tabs
  * array de containers


## Personalização

### Adicionar containers

```javascript
  var containersArr = [
    $('.w-section__container-center[data-module=" *Alterar* "]'),
    // Adicionar Containers necessários.
  ]
```

*****

### Alterar tab inicial

```javascript
    var showTab = 0;
```

*****

### Alterar class das tabs

```javascript
  var tabClass = $('. *Alterar* ');
```

*****

### Alterar class de active Tab ou Container

```javascript
  // Escolher active class
  var activeTabClass = 'active-tab';
  var activeContainerClass = 'active-container';
```

### Alterar propriedades do slider criado

Alterar a class onde é criado do Swiper, para mais informações: [Api do Swiper](https://idangero.us/swiper/api/)

```javascript
    // Criação do slider
  // Alterar classe de de iniciar slider
  var sliderTabs = new Swiper('.slider-tabs', {
    direction: 'horizontal',
    loop: false,
    slidesPerView:4,
    spaceBetween: 10,
    breakpoints: {
      640: {
        slidesPerView: 2,
        centeredSlides: false,
        loop: false,
        spaceBetween: 5
      }
    }
  })
```