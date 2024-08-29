---
meta:
  title: Product Lists
  description: Use these MAFUI product list components to build storefront and category pages for your online store with images, prices, and links to more details or purchase options. These components are designed and built by the MAFUI team, and include a variety of different styles and layouts.
layout: component
---

## Examples

### Mall of the Emirates Card

```html:preview
<div class="product-grid moe-style">
  <div class="product-row">
<mf-card class="card-overview">
  <div class="image-container">
    <img
      slot="image"
      src="https://dw4gwhhv7uqc1.cloudfront.net/catalog%2FSeller_36472%2F66b9655372450.jpg"
      alt="Men Basic Joggers With Side Pockets"
    />
    <div class="heart-icon-container">
      <mf-icon src="/assets/images/heart.svg" class="heart-icon"></mf-icon>
    </div>
    <div class="view-details">VIEW DETAILS</div>
  </div>
  <div class="product-info">
    <span class="brand">Carter & White</span><br>
    <span class="product-name">Men Masha Round Neck Pima Cotton Tshirt</span><br>
    <span class="price">AED 675.00</span>
  </div>
</mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://dw4gwhhv7uqc1.cloudfront.net/catalog%2FSeller_39515%2F66a1105ee5a37.jpg"
          alt="Merino Wool Sweater"
        />
      <div class="heart-icon-container">
        <mf-icon src="/assets/images/heart.svg" class="heart-icon"></mf-icon>
      </div>
        <div class="view-details">VIEW DETAILS</div>
      </div>
      <div class="product-info">
        <span class="brand">Brooks Brothers</span><br>
        <span class="product-name">Golden Fleece® Stretch Supima® Long-Sleeve</span><br>
        <span class="price">AED 495.00</span>
      </div>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://dw4gwhhv7uqc1.cloudfront.net/catalog%2FSeller_39515%2F66af8ea296a86.jpg"
          alt="Men Basic Joggers With Side Pockets"
        />
        <div class="heart-icon-container">
          <mf-icon src="/assets/images/heart.svg" class="heart-icon"></mf-icon>
        </div>
        <div class="view-details">VIEW DETAILS</div>
      </div>
      <div class="product-info">
        <span class="brand">That</span><br>
        <span class="product-name">Paul Smith Tapered Fit Jeans</span><br>
        <span class="price">AED 625.00</span>
      </div>
    </mf-card>

  </div>

  <div class="product-row">
    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://dw4gwhhv7uqc1.cloudfront.net/catalog%2FSeller_39515%2F66a1105ee3398.jpg"
          alt="Denim Jacket"
        />
        <div class="heart-icon-container">
          <mf-icon src="/assets/images/heart.svg" class="heart-icon"></mf-icon>
        </div>
        <div class="view-details">VIEW DETAILS</div>
      </div>
      <div class="product-info">
        <span class="brand">Brooks Brothers</span><br>
        <span class="product-name">Regent Classic-Fit Merino Wool </span><br>
        <span class="price">2,449.00 AED</span>
      </div>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://dw4gwhhv7uqc1.cloudfront.net/catalog%2FSeller_36472%2F66b965536f735.jpg"
          alt="Silk Tie"
        />
        <div class="heart-icon-container">
          <mf-icon src="/assets/images/heart.svg" class="heart-icon"></mf-icon>
        </div>
        <div class="view-details">VIEW DETAILS</div>
      </div>
      <div class="product-info">
        <span class="brand">Brooks Brothers</span><br>
        <span class="product-name">Silk Repp Stripe Tie Shirt BLK</span><br>
        <span class="price">299.00 AED</span>
      </div>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://dw4gwhhv7uqc1.cloudfront.net/catalog%2FSeller_39401%2F6666a9eab98ea.jpg"
          alt="Casual Sneakers"
        />
        <div class="heart-icon-container">
          <mf-icon src="/assets/images/heart.svg" class="heart-icon"></mf-icon>
        </div>
        <div class="view-details">VIEW DETAILS</div>
      </div>
      <div class="product-info">
        <span class="brand">Levi's</span><br>
        <span class="product-name">L-Pack Large Elevation Backpack</span><br>
        <span class="price">399.00 AED</span>
      </div>
    </mf-card>
  </div>
</div>

<style>
  .product-grid {
    display: flex;
    flex-direction: column;
    gap: 30px;
  }

  .moe-style .product-info {
    margin-top: 24px;
  }

  .moe-style .product-info .brand {
    text-transform: uppercase;
    font-size: 12px;
    letter-spacing: 2px;
    color: #333;
    font-weight: 500;
  }

  .moe-style .product-info .product-name {
    font-size: 20px;
    letter-spacing: -0.5px;
    color: #000;
    font-weight: 500;
    line-height: 28px; 
    font-family: var(--mf-font-serif)
  }

  .moe-style .product-info .price {
    font-size: 14px;
    color: #333;
  }

  .product-row {
    display: flex;
    justify-content: space-between;
    gap: 30px;
  }

  .card-overview {
    flex: 1;
    max-width: calc(33.333% - 20px);
    display: flex;
    flex-direction: column;
  }

  .moe-style .image-container {
    border: 1px solid #f5f5f5;
  }

  .image-container {
    position: relative;
    overflow: hidden;
    aspect-ratio: 3 / 4;
    background-color: #f0f0f0;
  }

  .moe-style .image-container img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center;
  }

  .heart-icon {
    position: absolute;
    top: 15px;
    right: 10px;
    color: black;
    background-color: #f2f3f3;
    border-radius: 50%;
    padding: 5px;
    z-index: 2;
  }

  .view-details {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    background-color: rgba(255, 255, 255, 0.9);
    color: black;
    text-align: center;
    padding: 10px;
    font-weight: 500;
    opacity: 0;
    visibility: hidden;
    transition: opacity 0.3s ease, visibility 0.3s ease;
  }

  .image-container:hover .view-details {
    opacity: 1;
    visibility: visible;
  }

  .badge {
    position: absolute;
    top: 0;
    left: 0;
  }

  @media (max-width: 1024px) {
    .product-row {
      flex-wrap: wrap;
    }
    .card-overview {
      max-width: calc(50% - 15px);
    }
  }

  @media (max-width: 640px) {
    .card-overview {
      max-width: 100%;
    }
  }
</style>
```

### Carrefour Card


```html:preview
<div class="product-grid c4-style">
  <div class="product-row">
    <mf-card class="card-overview">
      <div class="image-container">
        <img src="https://cdn.mafrservices.com/sys-master-root/h24/h03/9533382852638/70968_main.jpg?im=Resize=1700?im=Resize=400" alt="Premium Beef Tenderloin" />
      </div>
      <div class="c4-content">
        <div class="price-container">
          <div class="price">
            <span class="amount">2</span>
            <div class="decimal-currency">
              <span class="decimal">.25</span>
              <span class="currency">AED</span>
            </div>
          </div>
          <mf-button class="add-button" circle>
            <mf-icon name="plus" style="font-size: 28px;height: 32px;"></mf-icon>
          </mf-button>
        </div>
        <h3 class="product-name">Carrot</h3>
        <p class="product-details">600g - Approx 12 pieces/Kg</p>
      </div>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img src="https://cdn.mafrservices.com/sys-master-root/he4/hec/12631674191902/489903_1.jpg?im=Resize=1700?im=Resize=400" alt="Premium Beef Tenderloin" />
      </div>
      <div class="c4-content">
        <div class="price-container">
          <div class="price">
            <span class="amount">3</span>
            <div class="decimal-currency">
              <span class="decimal">.45</span>
              <span class="currency">AED</span>
            </div>
          </div>
          <mf-button class="add-button" circle>
            <mf-icon name="plus" style="font-size: 28px;height: 32px;"></mf-icon>
          </mf-button>
        </div>
        <h3 class="product-name">Clementine</h3>
        <p class="product-details">600g - Approx 10 pieces/Kg</p>
      </div>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img src="https://cdn.mafrservices.com/sys-master-root/h45/h8a/12631670456350/446302_main.jpg?im=Resize=1700?im=Resize=400" alt="Lean Ground Turkey" />
      </div>
      <div class="c4-content">
        <div class="price-container">
          <div class="price">
            <span class="amount">13</span>
            <div class="decimal-currency">
              <span class="decimal">.70</span>
              <span class="currency">AED</span>
            </div>
          </div>
          <mf-button class="add-button" circle>
            <mf-icon name="plus" style="font-size: 28px;height: 32px;"></mf-icon>
          </mf-button>
        </div>
        <h3 class="product-name">Clementine with Leaves</h3>
        <p class="product-details">500g - Approx 12 pieces/Kg</p>
      </div>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img src="https://cdn.mafrservices.com/sys-master-root/h8c/h06/9533382950942/71399_main.jpg?im=Resize=1700?im=Resize=400" alt="Grass-Fed Lamb Chops" />
      </div>
      <div class="c4-content">
        <div class="price-container">
          <div class="price">
            <span class="amount">2</span>
            <div class="decimal-currency">
              <span class="decimal">.30</span>
              <span class="currency">AED</span>
            </div>
          </div>
          <mf-button class="add-button" circle>
            <mf-icon name="plus" style="font-size: 28px;height: 32px;"></mf-icon>
          </mf-button>
        </div>
        <h3 class="product-name">Banana</h3>
        <p class="product-details">600g - Approx 5 pieces/kg</p>
      </div>
    </mf-card>
  </div>

  <div class="product-row">
    <mf-card class="card-overview">
      <div class="image-container">
        <img src="https://cdn.mafrservices.com/sys-master-root/h8e/h3c/62582488596510/449729_main.jpg?im=Resize=1700?im=Resize=400" alt="Organic Chicken Breast" />
      </div>
      <div class="c4-content">
        <div class="price-container">
          <div class="price">
            <span class="amount">2</span>
            <div class="decimal-currency">
              <span class="decimal">.40</span>
              <span class="currency">AED</span>
            </div>
          </div>
          <mf-button class="add-button" circle>
            <mf-icon name="plus" style="font-size: 28px;height: 32px;"></mf-icon>
          </mf-button>
        </div>
        <h3 class="product-name">Cucumber</h3>
        <p class="product-details">500g - Approx 9 pieces/kg</p>
      </div>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img src="https://cdn.mafrservices.com/sys-master-root/h77/h80/12631670718494/446434_main.jpg?im=Resize=1700?im=Resize=400" alt="Wild-Caught Salmon Fillet" />
      </div>
      <div class="c4-content">
        <div class="price-container">
          <div class="price">
            <span class="amount">2</span>
            <div class="decimal-currency">
              <span class="decimal">.48</span>
              <span class="currency">AED</span>
            </div>
          </div>
          <mf-button class="add-button" circle>
            <mf-icon name="plus" style="font-size: 28px;height: 32px;"></mf-icon>
          </mf-button>
        </div>
        <h3 class="product-name">Lemon</h3>
        <p class="product-details">500g - Approx 8 pieces/kg</p>
      </div>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img src="https://cdn.mafrservices.com/sys-master-root/h6d/he2/13754262978590/1767482_main.jpg?im=Resize=1700?im=Resize=400" alt="Premium Wagyu Beef Steak" />
      </div>
      <div class="c4-content">
        <div class="price-container">
          <div class="price">
            <span class="amount">1</span>
            <div class="decimal-currency">
              <span class="decimal">.48</span>
              <span class="currency">AED</span>
            </div>
          </div>
          <mf-button class="add-button" circle>
            <mf-icon name="plus" style="font-size: 28px;height: 32px;"></mf-icon>
          </mf-button>
        </div>
        <h3 class="product-name">Tomato</h3>
        <p class="product-details">500g - Approx 7 pieces/kg</p>
      </div>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img src="https://cdn.mafrservices.com/sys-master-root/h2f/hfc/15843619307550/446052_main.jpg?im=Resize=1700?im=Resize=400" alt="Premium Wagyu Beef Steak" />
      </div>
      <div class="c4-content">
        <div class="price-container">
          <div class="price">
            <span class="amount">4</span>
            <div class="decimal-currency">
              <span class="decimal">.48</span>
              <span class="currency">AED</span>
            </div>
          </div>
          <mf-button class="add-button" circle>
            <mf-icon name="plus" style="font-size: 28px;height: 32px;"></mf-icon>
          </mf-button>
        </div>
        <h3 class="product-name">Pink Lady Apple</h3>
        <p class="product-details">500g - Approx 6 pieces/kg</p>
      </div>
    </mf-card>

  </div>
</div>

<style>
  .c4-style .product-row {
    gap: 0;
  }

  .c4-style.product-grid {
    gap: 15px;
  }

  .c4-style .card-overview {
    max-width: 33.33%;
  }

  .c4-style .card-overview {
    border-radius: 16px;
    overflow: hidden;
    width: calc(33.333% - 14px);
    border: 1px solid rgb(239, 239, 239);
  }

  .c4-style .image-container {
    aspect-ratio: 1 / 1;
    background-color: #f0f0f0;
  }

  .c4-style .image-container img {
    width: 100%;
    height: 100%;
    object-fit: contain;
    object-position: center;
    padding: 0 11px;
    background: #fff;
  }

  .c4-style .c4-content {
    padding: 12px 12px 65px 12px;
  }

  .c4-style .price-container {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    margin-bottom: 10px;
  }

  .c4-style .price {
    font-weight: bold;
    display: flex;
    align-items: flex-start;
    line-height: 1;
  }

  .c4-style .price .amount {
    font-size: 20px;
    line-height: 0.9;
  }

  .c4-style .price .decimal-currency {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    margin-left: 2px;
  }

  .c4-style .price .decimal {
    font-size: 10px;
    font-weight:bold;
  }

  .c4-style .price .currency {
    font-size: 7px;
    color: #000;
    font-weight: 300;
  }

  .c4-style .product-name {
    font-size: 14px;
    font-weight: 400;
    margin: 0;
    line-height: 1.2;
  }

  .c4-style .product-details {
    font-size: 12px;
    color: #666;
    margin: 2px 0 0 0;
    line-height: 1.2;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }

  .c4-style mf-button.add-button::part(base) {
    background-color: #0f5aa7;
    border:none;
    color: #fff;
    height: 32px;
    width: 32px;
    min-height: 32px;
    margin-top: -60px;
  }
</style>
```


### THAT Concept Store Card

```html:preview
<div class="product-grid that-style">
  <div class="product-row">
    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://api-prod.thatconceptstore.com/medias/-original-U9060AAAM-NEWB-BLACK-001-1.webp-convert-600x800?context=bWFzdGVyfGF6dXJlaW1hZ2VzfDE0NzMyfGltYWdlL3dlYnB8YURZd0wyaGtZUzh4TVRVek56TXpOek00TkRrNU1DOHZiM0pwWjJsdVlXd3ZWVGt3TmpCQlFVRk5YMDVGVjBKZlFreEJRMHNnTURBeFh6RXVkMlZpY0Y5amIyNTJaWEowTFRZd01IZzRNREF8M2E1N2JmZmIwMTIwZTBjNGJhZjIzMmE4ZTc0NGQ3NGQyMTc4ZDM4ZWNjYzk4YWNmYmYwMmJkYWVkY2NiYmYxMg"
          alt="Dom Rebel Splash Knit Hoodie"
        />
        <div class="heart-icon"><mf-icon name="heart"></mf-icon></div>
      </div>

      <div class="product-info">
        <strong>New Balance</strong>
        <span class="product-name">9060 Low Top Sneakers</span>
        <span class="price">AED 799</span>
      </div>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://api-prod.thatconceptstore.com/medias/-original-6198434-ONRU-All-White-1.webp-convert-600x800?context=bWFzdGVyfGF6dXJlaW1hZ2VzfDE0MjA0fGltYWdlL3dlYnB8YURobEwyZ3pOaTh4TVRRMU5qUXhOREk0TlRnMU5DOHZiM0pwWjJsdVlXd3ZOakU1T0RRek5GOVBUbEpWWDBGc2JDQlhhR2wwWlY4eExuZGxZbkJmWTI5dWRtVnlkQzAyTURCNE9EQXd8ZWM1YjdjMzA2M2Q0Mjc5YmI0NTMzNGZlODI0YjhlZjEwZWM4MDdjZmM4NWU2Yzc0ZGE5YjVlYzdmNzlkODE5Mw"
          alt="LEGO Cooper's Robot Dinosaur C-Rex"
        />
        <div class="heart-icon"><mf-icon name="heart"></mf-icon></div>
      </div>

      <div class="product-info">
        <strong>ON</strong>
        <span class="product-name">Cloudmonster Sneakers</span>
        <span class="price">AED 875</span>
      </div>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://api-prod.thatconceptstore.com/medias/-original-GNS19001B-AFHM-B-Black-On-1.webp-convert-600x800?context=bWFzdGVyfGF6dXJlaW1hZ2VzfDIxNzQ2fGltYWdlL3dlYnB8YURFNEwyZzJPQzh4TVRJM05qUXhNRGM0TVRjeU5pOHZiM0pwWjJsdVlXd3ZSMDVUTVRrd01ERkNYMEZHU0UxZlFpQkNiR0ZqYXlCUGJsOHhMbmRsWW5CZlkyOXVkbVZ5ZEMwMk1EQjRPREF3fDE2NzZhMWQwNjYyOTJlOWFkYzFjYzNlMWUxODMzZGYzYWM3MDBjOGUwZDlkZGJhNDEwMGVjNzI5Mjc4MzQ0NmE"
          alt="LEGO Izzie's Dream Animals"
        />
        <div class="heart-icon"><mf-icon name="heart"></mf-icon></div>
      </div>

      <div class="product-info">
        <strong>Azza Fahmy</strong>
        <span class="product-name">Reversible Necklace</span>
        <span class="price">AED 1,600</span>
      </div>
    </mf-card>
  </div>
  <div class="product-row">
    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://api-prod.thatconceptstore.com/medias/-original-2513-DOMR-Grey-1.webp-convert-600x800?context=bWFzdGVyfGF6dXJlaW1hZ2VzfDUyNDc0fGltYWdlL3dlYnB8YURnd0wyZzBNeTh4TVRVM05qVTBOREF3TWpBM09DOHZiM0pwWjJsdVlXd3ZNalV4TTE5RVQwMVNYMGR5WlhsZk1TNTNaV0p3WDJOdmJuWmxjblF0TmpBd2VEZ3dNQXw4ODQzZDIxNDNhOWNjZjBkODFhZWZhZWZjZWQ2YTc4YTUzOTI0MGZmOTczMmY4NWMzMGM0MjkwYzQ2ZDgzYjQx"
          alt="LEGO Castle Nocturnia"
        />
        <div class="heart-icon"><mf-icon name="heart"></mf-icon></div>
        <div class="badges">
          <mf-badge variant="warning">Exclusive</mf-badge>
          <mf-badge variant="success">New</mf-badge>
        </div>
      </div>

      <div class="product-info">
        <strong>Dom Rebel</strong>
        <span class="product-name">Splash Knit Hoodie</span>
        <span class="price">AED 1,600</span>
      </div>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://api-prod.thatconceptstore.com/medias/-original-JC4741PE1-JUNJ-WHITE-1.webp-convert-600x800?context=bWFzdGVyfGF6dXJlaW1hZ2VzfDEyNDAyfGltYWdlL3dlYnB8YURrMUwyZzJZUzh4TVRZeE16WTFOVGcxT1RJek1DOHZiM0pwWjJsdVlXd3ZTa00wTnpReFVFVXhYMHBWVGtwZlYwaEpWRVZmTVM1M1pXSndYMk52Ym5abGNuUXROakF3ZURnd01BfDhiODRkYzMzOTU4MzVkMTk5YTZkYjY5NTdhMTA0YjMwNWVmMDdiOTU0Njg4NGRiOTVlNDM1ZTc5NjMxNzgyZGU"
          alt="LEGO Cooper's Robot Dinosaur C-Rex"
        />
        <div class="heart-icon"><mf-icon name="heart"></mf-icon></div>
      </div>

      <div class="product-info">
        <strong>Juun.J</strong>
        <span class="product-name">Essential Long Sleeve</span>
        <span class="price">AED 500</span>
      </div>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://api-prod.thatconceptstore.com/medias/-original-JC4921PD1-JUNJ-Black-1.webp-convert-600x800?context=bWFzdGVyfGF6dXJlaW1hZ2VzfDMxNTI4fGltYWdlL3dlYnB8YUdJMEwyaGpZUzh4TVRZeE16WTNPVE15TVRFeE9DOHZiM0pwWjJsdVlXd3ZTa00wT1RJeFVFUXhYMHBWVGtwZlFteGhZMnRmTVM1M1pXSndYMk52Ym5abGNuUXROakF3ZURnd01BfDNmNjlkZmIyYjE3N2FkMDAwMjQ0ZDc3MzFiNTA1YWM3ZTUzNDE1ZDJjMWU0MjMyNjVmMjM4ZTcxODA5NjE2MzE"
          alt="LEGO Izzie's Dream Animals"
        />
        <div class="heart-icon"><mf-icon name="heart"></mf-icon></div>
      </div>

      <div class="product-info">
        <strong>Juun.J</strong>
        <span class="product-name">Full Side-zip Destroyed</span>
        <span class="price">AED 600</span>
      </div>
    </mf-card>
  </div>
</div>

<style>
  .that-style .card-overview {
    border: none;
    box-shadow: none;
    padding: 0;
  }

  .that-style .image-container {
    position: relative;
    overflow: hidden;
  }

  .that-style .image-container img {
    width: 100%;
    height: auto;
    display: block;
  }

  .that-style .heart-icon {
    position: absolute;
    top: 10px;
    right: 10px;
    opacity: 0;
    transition: opacity 0.3s ease;
    background: transparent;
  }

  .that-style .card-overview:hover .heart-icon {
    opacity: 1;
  }

  .that-style .product-info {
    text-align: center;
    padding: 10px 0;
  }

  .that-style .product-info strong {
    display: block;
    font-size: 14px;
    margin-bottom: 5px;
    font-weight: 700;
  }

  .that-style .product-name {
    display: block;
    font-size: 14px;
    color: #5b5b5b;
    margin-bottom: 5px;
    font-weight: 500;
  }

  .that-style .price {
    display: block;
    font-size: 14px;
    font-weight: 500;
  }

  .that-style .card-overview:hover .image-container img {
      border: 2px solid #ffc81b;
      box-sizing: border-box;
    }
</style>
```

### LEGO Card

```html:preview
<div class="product-grid lego-style">
  <div class="product-row">
    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://api.lego.me/medias/-original-75398-1.jpg-convert-900x600?context=bWFzdGVyfGF6dXJlaW1hZ2VzfDM0NjY2fGltYWdlL2pwZWd8YURoaEwyaGlOQzh4TVRVM056QTJNalExTnpNM05DOHZiM0pwWjJsdVlXd3ZOelV6T1RoZk1TNXFjR2RmWTI5dWRtVnlkQzA1TURCNE5qQXd8NmYxM2M4YWQzYzMxMDFhMThmN2E0MjgwYThhMTZjMTBiNWNhNzI1NjhhYjkxNDk5NmI2NjkwODkzMjI2MWViMQ"
          alt="LEGO Castle Nocturnia"
        />
        <div class="heart-icon"><mf-icon name="heart"></mf-icon></div>
      </div>
      <h3 class="product-name">LEGO® C-3PO™</h3>
      <p class="product-price">AED 649</p>
      <mf-button class="add-to-bag" pill>
        <mf-icon src="/assets/images/minicart-icon.svg" class="bag-icon"></mf-icon>
        <span>Add to Bag</span> 
      </mf-button>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://api.lego.me/medias/-original-43247-1.jpg-convert-900x600?context=bWFzdGVyfGF6dXJlaW1hZ2VzfDQwNzAwfGltYWdlL2pwZWd8YUdKbUwyZzFOUzh4TVRReU5ESTVPRFEyTnpNMU9DOHZiM0pwWjJsdVlXd3ZORE15TkRkZk1TNXFjR2RmWTI5dWRtVnlkQzA1TURCNE5qQXd8NjljZjA2ZGY5MDg0NWM3MmViMDg1MzExMDRkOGVjOGY1ZjY4OTA2Nzk3ZjRmZmYxMGQ3YTI3NmZmOWUyYzFkMw"
          alt="LEGO Cooper's Robot Dinosaur C-Rex"
        />
        <div class="heart-icon"><mf-icon name="heart"></mf-icon></div>
      </div>

      <h3 class="product-name">LEGO® Young Simba the Lion</h3>
      <p class="product-price">AED 559</p>
        <mf-button class="add-to-bag" pill>
          <mf-icon src="/assets/images/minicart-icon.svg" class="bag-icon"></mf-icon>
          <span>Add to Bag</span> 
        </mf-button>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://api.lego.me/medias/-original-42173-1.jpg-convert-900x600?context=bWFzdGVyfGF6dXJlaW1hZ2VzfDU3NDg1fGltYWdlL2pwZWd8YUdNd0wyZ3haQzh4TVRVM05qazFOamcwTmpFeE1DOHZiM0pwWjJsdVlXd3ZOREl4TnpOZk1TNXFjR2RmWTI5dWRtVnlkQzA1TURCNE5qQXd8NjQ0ZmMyYjQ0MTRlYWZmYTM0MTI3MDBiYWVhNGM1NDFjMjZkN2JmZWVmMjE2MTIwYmE2MjkwOWFmM2VmMTRjMA"
          alt="LEGO Izzie's Dream Animals"
        />
        <div class="heart-icon"><mf-icon name="heart"></mf-icon></div>
      </div>

      <h3 class="product-name">LEGO® Koenigsegg Jesko Grey</h3>
      <p class="product-price">AED 239</p>
        <mf-button class="add-to-bag" pill>
          <mf-icon src="/assets/images/minicart-icon.svg" class="bag-icon"></mf-icon>
          <span>Add to Bag</span> 
        </mf-button>
    </mf-card>
  </div>
   <div class="product-row">
    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://api.lego.me/medias/-original-75389-1.jpg-convert-900x600?context=bWFzdGVyfGF6dXJlaW1hZ2VzfDc3MDQyfGltYWdlL2pwZWd8YURnekwyZzBPQzh4TVRVM056QTBOVEU0T0RZek9DOHZiM0pwWjJsdVlXd3ZOelV6T0RsZk1TNXFjR2RmWTI5dWRtVnlkQzA1TURCNE5qQXd8YzlmOGQ1M2Y5NWNhZjFkYTUzYTRiYzdhZjE2ODNiOTc2ZDJjNDVkMDc2YjBmOGE0MWZhMTllNGExZjk3N2YyYg"
          alt="LEGO Castle Nocturnia"
        />
        <div class="heart-icon"><mf-icon name="heart"></mf-icon></div>
      </div>

      <h3 class="product-name">LEGO® The Dark Falcon</h3>
      <p class="product-price">AED 699</p>
        <mf-button class="add-to-bag" pill>
          <mf-icon src="/assets/images/minicart-icon.svg" class="bag-icon"></mf-icon>
          <span>Add to Bag</span> 
        </mf-button>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://api.lego.me/medias/-original-42184-1.jpg-convert-900x600?context=bWFzdGVyfGF6dXJlaW1hZ2VzfDY1MDEzfGltYWdlL2pwZWd8YURkbEwyaGtPQzh4TVRVM05qazRNalEzTURZNE5pOHZiM0pwWjJsdVlXd3ZOREl4T0RSZk1TNXFjR2RmWTI5dWRtVnlkQzA1TURCNE5qQXd8ZDZmZDE3MmU4MDI4YjU2MzM4ZjU0YjU2YTQzNjBiOWU3YzJkNjBmZTJhODc4Y2I2NjFmN2JjMmExNDQ4YmRkNA"
          alt="LEGO Cooper's Robot Dinosaur C-Rex"
        />
        <div class="heart-icon"><mf-icon name="heart"></mf-icon></div>
      </div>

      <h3 class="product-name">LEGO® Koenigsegg Jesko</h3>
      <p class="product-price">AED 649</p>
        <mf-button class="add-to-bag" pill>
          <mf-icon src="/assets/images/minicart-icon.svg" class="bag-icon"></mf-icon>
          <span>Add to Bag</span> 
        </mf-button>
    </mf-card>

    <mf-card class="card-overview">
      <div class="image-container">
        <img
          slot="image"
          src="https://api.lego.me/medias/-original-76923-1.jpg-convert-900x600?context=bWFzdGVyfGF6dXJlaW1hZ2VzfDcwMzE1fGltYWdlL2pwZWd8YURkbEwyZzFaQzh4TVRReU5EVXlNak16T0RNek5DOHZiM0pwWjJsdVlXd3ZOelk1TWpOZk1TNXFjR2RmWTI5dWRtVnlkQzA1TURCNE5qQXd8ZjQyMGY1ZTA4NzU5NmRiNGQ5NzY4ODMwYTFkNDY4NWNiNDY3MzY5YmQyODdlNGFkMDAyNzlhZTgyYjJhNWZkYw"
          alt="LEGO Izzie's Dream Animals"
        />
        <div class="heart-icon"><mf-icon name="heart"></mf-icon></div>
      </div>

      <h3 class="product-name">LEGO® Lamborghini Lambo V12</h3>
      <p class="product-price">AED 119</p>
        <mf-button class="add-to-bag" pill>
          <mf-icon src="/assets/images/minicart-icon.svg" class="bag-icon"></mf-icon>
          <span>Add to Bag</span> 
        </mf-button>
    </mf-card>
  </div>
</div>

<style>

  .lego-style .product-row {
    gap: 0;
  }

  .lego-style.product-grid {
    gap: 0;
    border: 1px solid #e0e0e0;
    overflow: hidden;
  }

  .lego-style .card-overview {
    max-width: 33.33%;
    border-right: 1px solid #e0e0e0;
    border-bottom: 1px solid #e0e0e0;
    box-sizing: border-box;
  }

  .lego-style .card-overview:last-child {
    border-right: none;
  }

  .lego-style .product-row:last-child .card-overview {
    border-bottom: none;
  }

  .lego-style.product-grid {
    gap: 0;
  }

  .lego-style .card-overview {
    max-width: 33.33%;
  }

  .lego-style .heart-icon {
    top: 10px;
    left: 10px;
    right: auto;
    height: 30px;
    width: 30px;
    text-align: center;
  }

  .lego-style .product-name {
    font-weight: 500;
    margin-top: 15px;
    margin-bottom: 0px;
    font-size:14px;
    display: inline-block;
    padding: 0 14px;
  }

  .lego-style .product-price {
    font-weight: 700;
    color: #000;
    font-size:14px;
    padding: 0 16px;
    margin-bottom: 0px;
  }

  .lego-style .image-container {
    background: #fff;
  }

  .lego-style .image-container img {
      max-height: 100%;
      width: 100%;
      height: 60%;
      object-fit: contain;
      position: absolute;
      top: 0;
      bottom: 0;
      margin: auto;
      padding: 0 30px;
  }

  .lego-style .add-to-bag {
    padding: 14px;
  }

  .bag-icon {
    font-size:18px;
  }

  .lego-style mf-button.add-to-bag::part(base) {
    background-color: #FD8023;
    border:none;
    width: 146px;
    height:44px;
    padding: 3px;
  }
  
  .add-to-bag * {
    color: #000;
    font-weight: 600;
  }
</style>
```