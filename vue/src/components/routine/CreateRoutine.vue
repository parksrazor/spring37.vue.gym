<template>
  <div>
    <v-card>
      <v-toolbar flat color="primary" dark>
        <v-toolbar-title>새 루틴 생성하는 방법</v-toolbar-title>
      </v-toolbar>
      <v-tabs vertical>
        <v-tab>
          <v-icon left>mdi-account</v-icon>주의사항 1
        </v-tab>
        <v-tab>
          <v-icon left>mdi-lock</v-icon>주의사항 2
        </v-tab>
        <v-tab>
          <v-icon left>mdi-access-point</v-icon>주의사항 3
        </v-tab>

        <v-tab-item>
          <v-card flat>
            <v-card-text>
              <p>Sed aliquam ultrices mauris. Donec posuere vulputate arcu. Morbi ac felis. Etiam feugiat lorem non metus. Sed a libero.</p>
              <p>Nam ipsum risus, rutrum vitae, vestibulum eu, molestie vel, lacus. Aenean tellus metus, bibendum sed, posuere ac, mattis non, nunc. Aliquam lobortis. Aliquam lobortis. Suspendisse non nisl sit amet velit hendrerit rutrum.</p>
            </v-card-text>
          </v-card>
        </v-tab-item>
        <v-tab-item>
          <v-card flat>
            <v-card-text>
              <p>Morbi nec metus. Suspendisse faucibus, nunc et pellentesque egestas, lacus ante convallis tellus, vitae iaculis lacus elit id tortor. Sed mollis, eros et ultrices tempus, mauris ipsum aliquam libero, non adipiscing dolor urna a orci. Curabitur ligula sapien, tincidunt non, euismod vitae, posuere imperdiet, leo. Nunc sed turpis.</p>

              <p>Suspendisse feugiat. Suspendisse faucibus, nunc et pellentesque egestas, lacus ante convallis tellus, vitae iaculis lacus elit id tortor. Proin viverra, ligula sit amet ultrices semper, ligula arcu tristique sapien, a accumsan nisi mauris ac eros. In hac habitasse platea dictumst. Fusce ac felis sit amet ligula pharetra condimentum.</p>

              <p>Sed consequat, leo eget bibendum sodales, augue velit cursus nunc, quis gravida magna mi a libero. Nam commodo suscipit quam. In consectetuer turpis ut velit. Sed cursus turpis vitae tortor. Aliquam eu nunc.</p>

              <p>Etiam ut purus mattis mauris sodales aliquam. Ut varius tincidunt libero. Aenean viverra rhoncus pede. Duis leo. Fusce fermentum odio nec arcu.</p>

              <p
                class="mb-0"
              >Donec venenatis vulputate lorem. Aenean viverra rhoncus pede. In dui magna, posuere eget, vestibulum et, tempor auctor, justo. Fusce commodo aliquam arcu. Suspendisse enim turpis, dictum sed, iaculis a, condimentum nec, nisi.</p>
            </v-card-text>
          </v-card>
        </v-tab-item>
        <v-tab-item>
          <v-card flat>
            <v-card-text>
              <p>Fusce a quam. Phasellus nec sem in justo pellentesque facilisis. Nam eget dui. Proin viverra, ligula sit amet ultrices semper, ligula arcu tristique sapien, a accumsan nisi mauris ac eros. In dui magna, posuere eget, vestibulum et, tempor auctor, justo.</p>

              <p
                class="mb-0"
              >Cras sagittis. Phasellus nec sem in justo pellentesque facilisis. Proin sapien ipsum, porta a, auctor quis, euismod ut, mi. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nam at tortor in tellus interdum sagittis.</p>
            </v-card-text>
          </v-card>
        </v-tab-item>
      </v-tabs>
    </v-card>

    <v-container fluid>
      <v-layout row wrap>
        <v-flex>
          <v-card>
            <v-tabs background-color="white" color="deep-purple accent-4" right>
              <v-tab>Landscape</v-tab>
              <v-tab>City</v-tab>
              <v-tab>Abstract</v-tab>
              <v-tab-item v-for="n in 3" :key="n">
                <v-container fluid>
                  <v-row>
                    <v-col v-for="i in 6" :key="i" cols="12" md="4">
                      <v-img
                        :src="`https://picsum.photos/500/300?image=${i * n * 5 + 10}`"
                        :lazy-src="`https://picsum.photos/10/6?image=${i * n * 5 + 10}`"
                        aspect-ratio="1"
                      ></v-img>
                    </v-col>
                  </v-row>
                </v-container>
              </v-tab-item>
            </v-tabs>
          </v-card>
        </v-flex>
        <v-flex>
          <v-col cols="8" sm="5">
            <v-text-field label="키"></v-text-field>
          </v-col>
          <v-col cols="8" sm="5">
            <v-text-field label="몸무게"></v-text-field>
          </v-col>
          <v-col cols="8" sm="5">
            <v-text-field label="체지방량"></v-text-field>
          </v-col>
          <v-col cols="8" sm="5">
            <v-text-field label="골격근량"></v-text-field>
          </v-col>
          <v-col cols="8" sm="5"></v-col>
        </v-flex>
        <v-flex>
          <v-card max-width="200">
            <v-img src="@/assets/img/protein.jpg"></v-img>
            <v-card-title>추천상품</v-card-title>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
  </div>
</template>
<script>
</script>
<style></style>