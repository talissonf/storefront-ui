<template>
  <div id="category">
    <div class="navbar">
      <div class="navbar__aside desktop-only">
        <h1 class="navbar__title">Categories</h1>
      </div>
      <div class="navbar__main">
        <SfButton
          class="navbar__filters-button"
          @click="isFilterSidebarOpen = true"
        >
          <SfIcon size="15px" style="margin-right: 10px;">
            <svg viewBox="0 0 18 18" xmlns="http://www.w3.org/2000/svg">
              <g clip-icon="url(#clip0)">
                <path
                  d="m2.461 6.9416e-6h-0.1786c-1.113 0.0021094-2.0151 0.90421-2.0173 2.018v0.17859c-0.001406 0.53649 0.21024 1.0512 0.58851 1.4316 0.37829 0.38039 0.89226 0.59414 1.4287 0.59555h0.1786c0.53859 0.0014 1.0547-0.21165 1.4358-0.59204 0.38039-0.38039 0.59344-0.89719 0.59203-1.4351v-0.17859c-0.0014-0.53649-0.21585-1.0505-0.59554-1.4295-0.3804-0.37829-0.89581-0.58991-1.4323-0.58851zm1.452 2.1965c0.00141 0.38531-0.15047 0.75585-0.42329 1.028-0.27281 0.27281-0.64265 0.42539-1.0287 0.42329h-0.1786c-0.3839-7.1e-4 -0.75164-0.15399-1.0223-0.4261-0.27-0.27281-0.42117-0.64125-0.41906-1.0252v-0.1786c7.03e-4 -0.79594 0.64616-1.4407 1.4414-1.4421h0.1786c0.3839-0.00211 0.75305 0.14906 1.0252 0.41976 0.27281 0.27 0.4261 0.63844 0.4268 1.0223v0.1786z"
                />
                <path
                  d="m9.0959 0h-0.19265c-1.1109 0.005625-2.0095 0.90634-2.0117 2.018v0.17859c-0.00281 1.1145 0.89719 2.0214 2.0117 2.0272h0.19265c1.1145-0.00562 2.0144-0.91265 2.0117-2.0272v-0.17859c-0.0021-1.1116-0.9007-2.0124-2.0117-2.018zm1.4421 2.1965h-7e-4c0.0022 0.3839-0.149 0.75235-0.4197 1.0252-0.27001 0.27211-0.63846 0.4254-1.0217 0.4261h-0.19265c-0.79524-0.00141-1.4407-0.64616-1.4414-1.4421v-0.17859c-0.00211-0.3839 0.14907-0.75235 0.41976-1.0252 0.27-0.27211 0.63845-0.4254 1.0216-0.4261h0.19265c0.79524 0.001406 1.4407 0.64616 1.4414 1.4421l7e-4 0.17859z"
                />
                <path
                  d="m15.718 6.9631e-6h-0.1786c-0.5364-0.0014063-1.0518 0.21024-1.4322 0.58851-0.3797 0.37899-0.5942 0.89296-0.5956 1.4295v0.17859c-0.0014 0.5379 0.2117 1.0547 0.5921 1.4351 0.3811 0.38039 0.8972 0.59344 1.4358 0.59204h0.1786c0.5364-0.00141 1.0504-0.21516 1.4287-0.59555s0.5899-0.89509 0.5885-1.4316v-0.17859c-0.0021-1.1138-0.9042-2.0158-2.0172-2.018h-1e-4zm1.4414 2.1965c0.0022 0.3839-0.149 0.75234-0.419 1.0252-0.2707 0.27211-0.6385 0.42539-1.0224 0.4261h-0.1786c-0.386 0.00211-0.7558-0.15047-1.0286-0.42329-0.2728-0.27211-0.4247-0.64265-0.4233-1.028v-0.1786c7e-4 -0.3839 0.154-0.75234 0.4268-1.0223 0.2721-0.2707 0.6412-0.42188 1.0251-0.41976h0.1786c0.7953 0.001406 1.4407 0.64616 1.4414 1.4421v0.1786z"
                />
                <path
                  d="m2.461 6.8921h-0.17859c-1.1138 0.00211-2.0165 0.90562-2.0173 2.0194v0.17859c0.002109 1.1138 0.90421 2.0158 2.0173 2.018h0.17859c0.53719 0.0014 1.0526-0.2103 1.433-0.5892 0.3804-0.379 0.59415-0.89369 0.59485-1.4302v-0.1786c-0.00141-0.53649-0.21586-1.0505-0.59555-1.4294-0.38039-0.37829-0.89579-0.58991-1.4323-0.58851v-7e-5zm1.452 2.1965c-0.0014 0.79524-0.64616 1.4407-1.4421 1.4414h-0.1786c-0.3839 0.0021-0.75305-0.149-1.0252-0.419-0.27211-0.27073-0.4254-0.63847-0.4261-1.0224v-0.1786c7.03e-4 -0.79594 0.64617-1.4407 1.4414-1.4421h0.17859c0.38461-0.00211 0.75375 0.14906 1.0259 0.42046 0.2728 0.2707 0.42609 0.63915 0.42609 1.023v0.17719z"
                />
                <path
                  d="m9.0959 6.8921h-0.19266c-1.1116 0.00562-2.0102 0.90774-2.0117 2.0194v0.17859c0.00211 1.1116 0.9007 2.0124 2.0117 2.018h0.19266c1.1117-0.0056 2.0103-0.9078 2.0117-2.0194v-0.17859c-0.0021-1.1116-0.9007-2.0124-2.0117-2.018zm1.4421 2.1965h-7e-4c0 0.79664-0.64542 1.4421-1.4414 1.4435h-0.19266c-0.79524-0.0014-1.4407-0.64612-1.4414-1.4421v-0.17859c0-0.79664 0.64546-1.4421 1.4414-1.4435h0.19266c0.79524 0.00141 1.4407 0.64616 1.4414 1.4421l7e-4 0.1786z"
                />
                <path
                  d="m15.717 6.8922h-0.1786c-0.5371-0.0014-1.0525 0.21024-1.4329 0.58921-0.3804 0.37899-0.5942 0.89367-0.5949 1.4302v0.17859c0.0014 0.53649 0.2159 1.0505 0.5956 1.4295 0.3804 0.3783 0.8958 0.5899 1.4322 0.5885h0.1786c1.1138-0.0021 2.0166-0.9056 2.0173-2.0194v-0.17859c-0.0021-1.1138-0.9042-2.0158-2.0173-2.018v7e-5zm1.4414 2.1965c-7e-4 0.79524-0.6461 1.4407-1.4414 1.4414h-0.1786c-0.3839 0.0021-0.753-0.1491-1.0251-0.4191-0.2728-0.27065-0.4261-0.63839-0.4268-1.0223v-0.17859c0.0014-0.79594 0.6462-1.4407 1.4421-1.4421h0.1786c0.3839-0.00211 0.753 0.14906 1.0259 0.42046 0.2721 0.27071 0.4253 0.63915 0.4253 1.023v0.17719z"
                />
                <path
                  d="m9.0959 13.786h-0.19266c-1.1109 5e-3 -2.0095 0.9064-2.0117 2.0173v0.1786c0.00211 1.1116 0.9007 2.0124 2.0117 2.018h0.19266c1.111-0.0057 2.0096-0.9064 2.0117-2.018v-0.1786c-0.0021-1.1109-0.9007-2.0124-2.0117-2.0173zm1.4421 2.1966l-7e-4 -7e-4c-7e-4 0.7959-0.64612 1.4407-1.4414 1.4421h-0.19266c-0.79524-0.0014-1.4407-0.6462-1.4414-1.4421v-0.1786c7e-4 -0.7953 0.64616-1.4407 1.4414-1.4414h0.19266c0.79524 7e-4 1.4407 0.6461 1.4414 1.4414l7e-4 0.1793z"
                />
              </g>
            </svg>
          </SfIcon>
          Filters
        </SfButton>
        <div class="navbar__sort desktop-only">
          <span class="navbar__label">Sort by:</span>
          <SfSelect class="sort-by" v-model="sortBy">
            <SfSelectOption
              v-for="option in sortByOptions"
              :key="option.value"
              :value="option.value"
              >{{ option.label }}</SfSelectOption
            >
          </SfSelect>
        </div>
        <div class="navbar__counter">
          <span class="navbar__label desktop-only">Products found: </span>
          <strong class="desktop-only">280</strong>
          <span class="navbar__label mobile-only">280 Items</span>
        </div>
        <div class="navbar__view desktop-only">
          <span>View </span>
          <SfIcon class="navbar__view-icon" size="10px">
            <svg viewBox="0 0 10 10">
              <rect width="2" height="2" fill="#1D1F22" />
              <rect y="4" width="2" height="2" fill="#1D1F22" />
              <rect y="8" width="2" height="2" fill="#1D1F22" />
              <rect x="4" width="2" height="2" fill="#1D1F22" />
              <rect x="4" y="4" width="2" height="2" fill="#1D1F22" />
              <rect x="4" y="8" width="2" height="2" fill="#1D1F22" />
              <rect x="8" width="2" height="2" fill="#1D1F22" />
              <rect x="8" y="4" width="2" height="2" fill="#1D1F22" />
              <rect x="8" y="8" width="2" height="2" fill="#1D1F22" />
            </svg>
          </SfIcon>
          <SfIcon class="navbar__view-icon" size="11px">
            <svg viewBox="0 0 11 10" fill="none">
              <rect width="11" height="2" fill="#BEBFC4" />
              <rect y="8" width="11" height="2" fill="#BEBFC4" />
              <rect y="4" width="7" height="2" fill="#BEBFC4" />
            </svg>
          </SfIcon>
        </div>
        <SfButton
          class="navbar__filters-button mobile-only"
          @click="isFilterSidebarOpen = true"
        >
          Sort by
          <SfIcon size="15px" style="margin-left: 10px;">
            <svg viewBox="0 0 12 16" xmlns="http://www.w3.org/2000/svg">
              <path
                d="M8.32809 15.2897L12 11.7644V12.2892L8.13547 16L4.27094 12.2892V11.7644L7.94285 15.2897V6.83165H8.32809L8.32809 15.2897ZM3.67191 0.710288L0 4.23556V3.71082L3.86453 0L7.72906 3.71082V4.23556L4.05715 0.710288V9.16835H3.67191L3.67191 0.710288Z"
              />
            </svg>
          </SfIcon>
        </SfButton>
      </div>
    </div>
    <div class="main">
      <div class="sidebar desktop-only">
        <SfAccordion :firstOpen="true">
          <template v-slot="{ selected }">
            <SfAccordionItem
              v-for="(accordion, i) in sidebarAccordion"
              :key="i"
              :header="accordion.header"
            >
              <template v-slot="{ handler }">
                <SfList>
                  <SfListItem v-for="(item, j) in accordion.items" :key="j">
                    <div
                      @click="
                        () => {
                          handler(item.label);
                        }
                      "
                    >
                      <SfMenuItem
                        class="menu-item"
                        :class="{
                          'menu-item--active': selected === item.label
                        }"
                        :label="item.label"
                        :count="item.count"
                      />
                    </div>
                  </SfListItem>
                </SfList>
              </template>
            </SfAccordionItem>
          </template>
        </SfAccordion>
      </div>
      <div class="products" style="">
        <div class="products__list">
          <SfProductCard
            v-for="(product, i) in products"
            :key="i"
            :title="product.title"
            :regular-price="product.price.regular"
            :special-price="product.price.special"
            :rating="product.rating.score"
            :isOnWishlist="product.isOnWishlist"
            @click:wishlist="
              () => {
                toggleWishlist(i);
              }
            "
            class="products__product-card"
          />
        </div>
        <SfPagination
          class="products__pagination desktop-only"
          :current="currentPage"
          @click="
            page => {
              this.currentPage = page;
            }
          "
          :total="4"
          :visible="5"
        />
      </div>
    </div>
    <SfSidebar
      :visible="isFilterSidebarOpen"
      @close="isFilterSidebarOpen = false"
      class="filters"
    >
      <h3 class="filters__title">Collection</h3>
      <SfFilter
        v-for="filter in filtersOptions.collection"
        :key="filter.value"
        :label="filter.label"
        :count="filter.count"
      />
      <h3 class="filters__title">Color</h3>
      <SfFilter
        v-for="filter in filtersOptions.color"
        :key="filter.value"
        :value="filter.value"
        :label="filter.label"
        :color="filter.color"
      />
      <h3 class="filters__title">Size</h3>
      <SfFilter
        v-for="filter in filtersOptions.size"
        :key="filter.value"
        :value="filter.value"
        :label="filter.label"
        :count="filter.count"
      />
      <h3 class="filters__title">Price</h3>
      <SfFilter
        v-for="filter in filtersOptions.price"
        :key="filter.value"
        :value="filter.value"
        :label="filter.label"
        :count="filter.count"
      />
      <h3 class="filters__title">Material</h3>
      <SfFilter
        v-for="filter in filtersOptions.material"
        :key="filter.value"
        :value="filter.value"
        :label="filter.label"
        :count="filter.count"
      />
      <div class="filters__buttons">
        <SfButton
          @click="isFilterSidebarOpen = false"
          class="sf-button--full-width"
          >Done</SfButton
        >
        <SfButton
          @click="clearAllFilters"
          class="sf-button--full-width filters__button-clear"
          >Clear all</SfButton
        >
      </div>
    </SfSidebar>
  </div>
</template>
<script>
import {
  SfSidebar,
  SfButton,
  SfList,
  SfIcon,
  SfMenuItem,
  SfFilter,
  SfProductCard,
  SfPagination,
  SfAccordion,
  SfSelect
} from "../../../../index.js";

export default {
  data() {
    return {
      currentPage: 1,
      sortBy: "price-up",
      isFilterSidebarOpen: true,
      filters: {
        color: [],
        collection: [],
        size: [],
        price: [],
        material: []
      },
      sortByOptions: [
        {
          value: "latest",
          label: "Latest"
        },
        {
          value: "price-up",
          label: "Price from low to high"
        },
        {
          value: "price-down",
          label: "Price from high to low"
        }
      ],
      sidebarAccordion: [
        {
          header: "Clothing",
          items: [
            { label: "All", count: "280" },
            { label: "Skirts", count: "23" },
            { label: "Sweaters", count: "54" },
            { label: "Dresses", count: "34" },
            { label: "T-shirts", count: "56" },
            { label: "Pants", count: "7" },
            { label: "Underwear", count: "12" }
          ]
        },
        {
          header: "Accesorries",
          items: [
            { label: "All", count: "280" },
            { label: "Skirts", count: "23" },
            { label: "Sweaters", count: "54" },
            { label: "Dresses", count: "34" },
            { label: "T-shirts", count: "56" },
            { label: "Pants", count: "7" },
            { label: "Underwear", count: "12" }
          ]
        },
        {
          header: "Shoes",
          items: [
            { label: "All", count: "280" },
            { label: "Skirts", count: "23" },
            { label: "Sweaters", count: "54" },
            { label: "Dresses", count: "34" },
            { label: "T-shirts", count: "56" },
            { label: "Pants", count: "7" },
            { label: "Underwear", count: "12" }
          ]
        }
      ],
      products: [
        {
          title: "Cream Beach Bag",
          image: "assets/storybook/homepage/productA.png",
          price: { regular: "$50.00", special: "$20.00" },
          rating: { max: 5, score: false },
          isOnWishlist: true
        },
        {
          title: "Cream Beach Bag",
          image: "assets/storybook/homepage/productB.png",
          price: { regular: "$50.00" },
          rating: { max: 5, score: 4 },
          isOnWishlist: false
        },
        {
          title: "Cream Beach Bag",
          image: "assets/storybook/homepage/productC.png",
          price: { regular: "$50.00" },
          rating: { max: 5, score: 4 },
          isOnWishlist: false
        },
        {
          title: "Cream Beach Bag",
          image: "assets/storybook/homepage/productA.png",
          price: { regular: "$50.00" },
          rating: { max: 5, score: 4 },
          isOnWishlist: false
        },
        {
          title: "Cream Beach Bag",
          image: "assets/storybook/homepage/productB.png",
          price: { regular: "$50.00" },
          rating: { max: 5, score: 4 },
          isOnWishlist: false
        },
        {
          title: "Cream Beach Bag",
          image: "assets/storybook/homepage/productC.png",
          price: { regular: "$50.00" },
          rating: { max: 5, score: 4 },
          isOnWishlist: false
        },
        {
          title: "Cream Beach Bag",
          image: "assets/storybook/homepage/productA.png",
          price: { regular: "$50.00" },
          rating: { max: 5, score: 4 },
          isOnWishlist: false
        },
        {
          title: "Cream Beach Bag",
          image: "assets/storybook/homepage/productB.png",
          price: { regular: "$50.00" },
          rating: { max: 5, score: 4 },
          isOnWishlist: false
        }
      ],
      filtersOptions: {
        collection: [
          { label: "Summer fly", value: "summer-fly", count: "10" },
          { label: "Best 2018", value: "best-2018", count: "23" },
          { label: "Your choice", value: "your-choice", count: "54" }
        ],
        color: [
          { label: "Red", value: "red", color: "#990611" },
          { label: "Black", value: "black", color: "#000000" },
          { label: "Yellow", value: "yellow", color: "#DCA742" },
          { label: "Blue", value: "blue", color: "#004F97" },
          { label: "Navy", value: "navy", color: "#656466" },
          { label: "White", value: "white", color: "#FFFFFF" }
        ],
        size: [
          { label: "Size 2 (XXS)", value: "xxs", count: "10" },
          { label: "Size 4-6 (XS)", value: "xs", count: "23" },
          { label: "Size 8-10 (S)", value: "s", count: "54" },
          { label: "Size 12-14 (M)", value: "m", count: "109" },
          { label: "Size 16-18 (L)", value: "l", count: "23" },
          { label: "Size 20-22(XL)", value: "xl", count: "12" },
          { label: "Size 24-26 (XXL)", value: "xxl", count: "2" }
        ],
        price: [
          { label: "Under $200", value: "under-200", count: "23" },
          { label: "Under $300", value: "under-300", count: "54" }
        ],
        material: [
          { label: "Cotton", value: "coton", count: "33" },
          { label: "Silk", value: "silk", count: "73" }
        ]
      }
    };
  },
  methods: {
    clearAllFilters() {
      const filters = {};
      const keys = Object.keys(this.filters);
      keys.forEach(key => {
        filters[key] = [];
      });
      this.filters = filters;
    },
    toggleWishlist(index) {
      this.products[index].isOnWishlist = !this.products[index].isOnWishlist;
    }
  },
  components: {
    SfButton,
    SfSidebar,
    SfIcon,
    SfList,
    SfFilter,
    SfProductCard,
    SfPagination,
    SfMenuItem,
    SfAccordion,
    SfSelect
  }
};
</script>
<style lang="scss" scoped>
@import "../../../css/variables";
@import "~@storefront-ui/shared/styles/helpers/visibility";

#category {
  box-sizing: border-box;
  max-width: 1240px;
  margin: auto;
  /*padding: 0 $spacer-big;
  @media screen and (min-width: $desktop-min) {
    padding: 0;
  }*/
}
.navbar {
  display: flex;
  padding: $spacer;
  border-top: 1px solid $c-border;
  border-bottom: 1px solid $c-border;
  @media screen and (min-width: $desktop-min) {
    padding: 0;
  }
  &__aside {
    display: flex;
    align-items: center;
    flex: 0 0 15%;
    padding: 0 $spacer-extra-big;
    border-right: 1px solid $c-border;
  }
  &__main {
    flex: 1;
    display: flex;
    align-items: center;
    font-size: $font-size-small-desktop;
  }
  &__title {
    padding: 0;
    font-size: $font-size-big-desktop;
    line-height: 2.23;
  }
  &__filters-button {
    display: flex;
    align-items: center;
    margin: 0;
    padding: 0;
    background: transparent;
    color: inherit;
    font-size: inherit;
    font-weight: 500;
    @media (min-width: $desktop-min) {
      margin: 0 0 0 $spacer-extra-big;
      font-weight: 400;
      text-transform: none;
    }
    svg {
      fill: $c-dark-primary;
      @media (min-width: $desktop-min) {
        fill: $c-gray-secondary;
      }
    }
    &:hover {
      color: $c-accent-primary;
      svg {
        fill: $c-accent-primary;
      }
    }
  }
  &__label {
    color: $c-gray-secondary;
  }
  &__sort {
    display: flex;
    align-items: center;
    margin-left: $spacer-extra-big;
    margin-right: auto;
  }
  &__counter {
    margin: auto;
    @media (min-width: $desktop-min) {
      margin-right: 0;
    }
  }
  &__view {
    display: flex;
    align-items: center;
    margin: 0 $spacer-extra-big;
    &-icon {
      margin-left: 10px;
    }
  }
}
.main {
  display: flex;
}
.sidebar {
  flex: 0 0 15%;
  padding: $spacer-extra-big;
  border-right: 1px solid $c-border;
}
.products {
  flex: 1;
  @media (min-width: $desktop-min) {
    margin: $spacer-big;
  }
  &__list {
    display: flex;
    flex-wrap: wrap;
  }
  &__product-card {
    flex: 0 0 50%;
    padding: $spacer;
    @media (min-width: $desktop-min) {
      flex: 0 0 25%;
      padding: $spacer-big;
    }
  }
  &__pagination {
    @media (min-width: $desktop-min) {
      margin-top: $spacer-extra-big;
    }
  }
}
.filters {
  &__title:not(:first-child),
  &__buttons {
    margin-top: $spacer-big * 3;
  }
  &__title {
    font-size: $font-size-big-desktop;
    line-height: 2.23;
  }
  &__button-clear {
    margin-top: 10px;
    background: $c-light-primary;
    color: #a3a5ad;
  }
}
.sort-by {
  flex: unset;
  width: 175px;
  /deep/ .sf-select__selected {
    padding: 10px;
  }
  /deep/ .sf-select-option {
    padding: 10px;
  }
}
.menu-item {
  &--active,
  &:hover {
    font-weight: 500;
    text-decoration: underline;
    cursor: pointer;
  }
}
</style>
