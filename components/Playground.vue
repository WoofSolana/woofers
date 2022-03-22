

<template>
  <div>
    <div class="container max-w-8xl m-auto">
      <div class="playground bg-gray-600 flex flex-col justify-center items-start m-4 py-8 px-4 rounded-lg">
        <div class="playground__title">WOOF Playground</div>
        <div class="playground__wrapper w-full py-8">
          <div class="playground__attributes">
            <div class="playground__attribute-wrapper">
              <div class="playground-select">


                <label for="Background" class="playground-select__label">
                  Background
                </label>
                <select v-model='selected'  class="playground-select__select">
                  <option v-for="option in backgrounds" :value="option.value" class="playground-select__option"> {{ option.text }} </option>
                </select>


              </div>
              <div  for="Background" class="playground-attribute">
                <div v-for="option in backgrounds" :value="option.value" class="playground-attribute__percentage"> {{ option.rarity }} </div>
                <div
                  class="playground-attribute__rarity playground-attribute__rarity--Common"
                >
                  Common
                </div>
              </div>
            </div>
            <div class="playground__attribute-wrapper">
              <div class="playground-select">
                <label for="Type" class="playground-select__label">Skin / Breed</label
                ><select id="Type" class="playground-select__select">
                  <option value="Brown" class="playground-select__option">
                    Terrier
                  </option>
                  <option value="Gold" class="playground-select__option">
                    Labrador
                  </option>
                  <option value="White" class="playground-select__option">
                    Retriever
                  </option>
                  <option value="Red" class="playground-select__option">
                    Beagle
                  </option>
                  <option value="Black" class="playground-select__option">
                    Ridgeback
                  </option>
                  <option value="Solana" class="playground-select__option">
                    Doberman
                  </option>
                  <option value="Solana" class="playground-select__option">
                    Alaskan
                  </option>
                  <option value="Solana" class="playground-select__option">
                    Golden
                  </option>
                  <option value="Solana" class="playground-select__option">
                    Woof
                  </option>
                  <option value="Solana" class="playground-select__option">
                    Skeleton
                  </option>
                </select>
              </div>
              <div class="playground-attribute">
                <div class="playground-attribute__percentage">17.10%</div>
                <div
                  class="playground-attribute__rarity playground-attribute__rarity--Common"
                >
                  Common
                </div>
              </div>
            </div>
            <div class="playground__attribute-wrapper">
              <div class="playground-select">
                <label for="Clothing" class="playground-select__label"
                  >Clothing</label
                ><select id="Clothing" class="playground-select__select">
                  <option value="None" class="playground-select__option">
                    None
                  </option>
                  <option value="Ying Yang" class="playground-select__option">
                    Ying Yang
                  </option>
                  <option
                    value="Orange Cosmo"
                    class="playground-select__option"
                  >
                    Orange Cosmo
                  </option>
                  <option value="Green Cosmo" class="playground-select__option">
                    Green Cosmo
                  </option>
                  <option
                    value="Eclipse Suit"
                    class="playground-select__option"
                  >
                    Eclipse Suit
                  </option>
                  <option value="Sun Suit" class="playground-select__option">
                    Sun Suit
                  </option>
                  <option value="Commander" class="playground-select__option">
                    Commander
                  </option>
                  <option value="Warrior" class="playground-select__option">
                    Warrior
                  </option>
                  <option value="Winter Suit" class="playground-select__option">
                    Winter Suit
                  </option>
                  <option value="Moon Suit" class="playground-select__option">
                    Moon Suit
                  </option>
                  <option
                    value="Neptune Suit"
                    class="playground-select__option"
                  >
                    Neptune Suit
                  </option>
                  <option
                    value="Captain Aperica"
                    class="playground-select__option"
                  >
                    Captain Aperica
                  </option>
                </select>
              </div>
              <div class="playground-attribute">
                <div class="playground-attribute__percentage">5.49%</div>
                <div
                  class="playground-attribute__rarity playground-attribute__rarity--Epic"
                >
                  Epic
                </div>
              </div>
            </div>
            <div class="playground__attribute-wrapper">
              <div class="playground-select">
                <label for="Mouth" class="playground-select__label">Mouth</label
                ><select id="Mouth" class="playground-select__select">
                  <option value="Normal" class="playground-select__option">
                    Normal
                  </option>
                  <option value="Cigar" class="playground-select__option">
                    Cigar
                  </option>
                  <option value="Pipe" class="playground-select__option">
                    Pipe
                  </option>
                  <option value="Bubblegum" class="playground-select__option">
                    Bubblegum
                  </option>
                </select>
              </div>
              <div class="playground-attribute">
                <div class="playground-attribute__percentage">22.86%</div>
                <div
                  class="playground-attribute__rarity playground-attribute__rarity--Epic"
                >
                  Epic
                </div>
              </div>
            </div>
            <div class="playground__attribute-wrapper">
              <div class="playground-select">
                <label for="Eyes" class="playground-select__label">Eyes</label
                ><select id="Eyes" class="playground-select__select">
                  <option value="Normal" class="playground-select__option">
                    Normal
                  </option>
                  <option
                    value="Moon Glasses"
                    class="playground-select__option"
                  >
                    Moon Glasses
                  </option>
                  <option value="Cyborg" class="playground-select__option">
                    Cyborg
                  </option>
                  <option value="One-eyed" class="playground-select__option">
                    One-eyed
                  </option>
                  <option value="Sunglasses" class="playground-select__option">
                    Sunglasses
                  </option>
                  <option value="Third Eye" class="playground-select__option">
                    Third Eye
                  </option>
                  <option
                    value="Cyclops Visor"
                    class="playground-select__option"
                  >
                    Cyclops Visor
                  </option>
                </select>
              </div>
              <div class="playground-attribute">
                <div class="playground-attribute__percentage">13.95%</div>
                <div
                  class="playground-attribute__rarity playground-attribute__rarity--Epic"
                >
                  Epic
                </div>
              </div>
            </div>
            <div class="playground__attribute-wrapper">
              <div class="playground-select">
                <label for="Head" class="playground-select__label">Head</label
                ><select id="Head" class="playground-select__select">
                  <option value="None" class="playground-select__option">
                    None
                  </option>
                  <option value="Blue Cap" class="playground-select__option">
                    Blue Cap
                  </option>
                  <option value="Black Cap" class="playground-select__option">
                    Black Cap
                  </option>
                  <option value="Moon Hat" class="playground-select__option">
                    Moon Hat
                  </option>
                  <option value="Eyes" class="playground-select__option">
                    Eyes
                  </option>
                  <option value="Captain Hat" class="playground-select__option">
                    Captain Hat
                  </option>
                  <option
                    value="Purple Mohawk"
                    class="playground-select__option"
                  >
                    Purple Mohawk
                  </option>
                  <option value="Horns" class="playground-select__option">
                    Horns
                  </option>
                  <option value="Red Mohawk" class="playground-select__option">
                    Red Mohawk
                  </option>
                  <option value="Band" class="playground-select__option">
                    Band
                  </option>
                  <option value="Unicorn" class="playground-select__option">
                    Unicorn
                  </option>
                  <option value="Slime" class="playground-select__option">
                    Slime
                  </option>
                  <option value="Among Apes" class="playground-select__option">
                    Among Apes
                  </option>
                  <option value="Ape Wars" class="playground-select__option">
                    Ape Wars
                  </option>
                </select>
              </div>
              <div class="playground-attribute">
                <div class="playground-attribute__percentage">2.88%</div>
                <div
                  class="playground-attribute__rarity playground-attribute__rarity--Mythic"
                >
                  Mythic
                </div>
              </div>
            </div>
          </div>
          <div class="playground__layers-wrapper">
            <div class="playground__layers">
              <div
                class="playground__layer"
                style="
                  background-image: url('');
                "
              ></div>
              <div
                class="playground__layer"
                style="
                  background-image: url('');
                "
              ></div>
              <div
                class="playground__layer"
                style="
                  background-image: url('');
                "
              ></div>
              <div
                class="playground__layer"
                style="
                  background-image: url('');
                "
              ></div>
              <div
                class="playground__layer"
                style="
                  background-image: url('');
                "
              ></div>
              <div
                class="playground__layer"
                style="
                  background-image: url('');
                "
              ></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
    import styling from "@/assets/css/main.css"
    import usage from "@/assets/js/main.js"
    import { teamCardSections } from "@/assets/data.js"
    export default {
        data() {
            return {
                selected: 'gold',
                backgrounds: [
                  { text: 'Sandy Gold', value: 'gold', image: 'assets/images/woofers/sandy.png', rarity: '50.00%' },
                  { text: 'East Bay Blue', value: 'blue', image: 'assets/images/woofers/blue.png', rarity: '40.00%' },
                  { text: 'Burgundy', value: 'burg', image: 'assets/images/woofers/burg.png', rarity: '9.00%' },
                  { text: 'East Bay Blue', value: 'night', image: 'assets/images/woofers/blue.png', rarity: '1.00%' }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    .playground {
        background-color: #1F1F1F;
        color: white;
    }

    .playground__attribute-wrapper {
        position: relative;
        background-color: #1A1A1A;
        margin-bottom: 1.5rem;
        padding: 0.5rem;
        border-radius: 0.5rem;
        width: 100%;
    }
    .playground-select {
        display: flex;
        flex-direction: column;
        width: 70%;
    }
    .playground-select__select {
        background-color: #121212;
        padding: 0.5rem;
    }
    .playground-select__label {
        padding-bottom: 0.5rem;
    }
        

        .playground-attribute__percentage {
            position: absolute;
            right: 1.5rem;
            top: 3rem;
        }

        .playground-attribute__rarity {
            position: absolute;
            top: -0.50rem;
            right: -0.1rem;
            background-color: blue;
            padding: 8px 16px 8px 16px;
            font-size: 10px;
            font-weight: 200;
            border-radius: 8px;
            letter-spacing: 1px;
            text-transform: uppercase;
        }
</style>
