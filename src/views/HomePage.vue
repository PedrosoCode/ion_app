<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Bem vindo</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-label class="ion-padding ion-text-center">
        <h1>Bem vindo de volta!</h1>
        <p>Escolha seu formato de acesso</p>
      </ion-label>

      <ion-card>
        <ion-segment>
          <ion-segment-button value="seg-login" content-id="seg-login">
            <ion-label>Login</ion-label>
          </ion-segment-button>
          <ion-segment-button value="seg-cadastro" content-id="seg-cadastro">
            <ion-label>Cadastro</ion-label>
          </ion-segment-button>
        </ion-segment>
        <ion-segment-view>
          <ion-segment-content id="seg-login" class="ion-align-items-end"><ion-grid>
              <ion-row>
                <ion-col>
                  <ion-input label="Usuário" label-placement="floating" fill="outline"
                    placeholder="Insira seu usuário"></ion-input>
                </ion-col>
              </ion-row>
              <ion-row>
                <ion-col>
                  <ion-input type="password" label="Password" value="NeverGonnaGiveYouUp" fill="outline">
                    <ion-input-password-toggle slot="end"></ion-input-password-toggle>
                  </ion-input>
                </ion-col>
              </ion-row>
              <ion-row>
                <ion-col>
                  <ion-list>
                    <ion-item>
                      <ion-select aria-label="Empresa" interface="popover" placeholder="Selecione a empresa">
                        <ion-select-option value="Empresa A">Empresa A</ion-select-option>
                        <ion-select-option value="Empresa B">Empresa B</ion-select-option>
                        <ion-select-option value="Empresa C">Empresa C</ion-select-option>
                      </ion-select>
                    </ion-item>
                  </ion-list>
                </ion-col>
              </ion-row>
            </ion-grid>
            <ion-grid>
              <ion-row class="ion-align-items-end">
                <ion-col>
                  <ion-button router-link="/about" router-direction="forward" expand="block">Logar</ion-button>
                </ion-col>
              </ion-row>
            </ion-grid>
          </ion-segment-content>
          <ion-segment-content id="seg-cadastro">
            <ion-grid>
              <ion-row>
                <ion-col>
                  <ion-input label="Usuário" label-placement="floating" fill="outline"
                    placeholder="Insira seu usuário"></ion-input>
                </ion-col>
              </ion-row>
              <ion-row>
                <ion-col>
                  <ion-input label="E-mail" label-placement="floating" fill="outline"
                    placeholder="Insira seu melhor E-mail"></ion-input>
                </ion-col>
              </ion-row>
              <ion-row>
                <ion-col>
                  <ion-input type="password" label="Password" value="NeverGonnaGiveYouUp" fill="outline">
                    <ion-input-password-toggle slot="end"></ion-input-password-toggle>
                  </ion-input>
                </ion-col>
              </ion-row>
              <ion-row>
                <ion-col>
                  <ion-list>
                    <ion-item>
                      <ion-select aria-label="Empresa" interface="popover" placeholder="Selecione a empresa">
                        <ion-select-option value="Empresa A">Empresa A</ion-select-option>
                        <ion-select-option value="Empresa B">Empresa B</ion-select-option>
                        <ion-select-option value="Empresa C">Empresa C</ion-select-option>
                      </ion-select>
                    </ion-item>
                  </ion-list>
                </ion-col>
              </ion-row>
              <ion-row class="ion-justify-content-center">
                <ion-col>
                  <ion-button router-link="/about" router-direction="forward" expand="block">Cadastrar</ion-button>
                </ion-col>
              </ion-row>
            </ion-grid></ion-segment-content>
        </ion-segment-view>
      </ion-card>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import {
  IonItem,
  IonSelect,
  IonSelectOption,
  IonList,
  IonInput,
  IonInputPasswordToggle,
  IonGrid,
  IonRow,
  IonCol,
  IonLabel,
  IonSegment,
  IonSegmentButton,
  IonSegmentContent,
  IonSegmentView,
  IonCard,
  IonTabs,
  IonTab,
  IonTabBar,
  IonTabButton,
  IonIcon,
  IonButton,
  IonContent,
  IonHeader,
  IonPage,
  IonTitle,
  IonToolbar,
} from "@ionic/vue";
</script>
