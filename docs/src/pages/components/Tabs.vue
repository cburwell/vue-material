<template>
  <page-content page-title="Components - Tabs">
    <docs-component>
      <div slot="description">
        <p>Tabs enable content organization at a high level, such as switching between views, data sets, or functional aspects of an app.</p>
        <p>The following classes can be applied to change the color palette:</p>
        <ul class="md-body-2">
          <li><code>md-accent</code></li>
          <li><code>md-warn</code></li>
          <li><code>md-transparent</code></li>
        </ul>
      </div>

      <div slot="api">
        <api-table name="md-tabs">
          <md-table slot="properties">
            <md-table-header>
              <md-table-row>
                <md-table-head>Name</md-table-head>
                <md-table-head>Type</md-table-head>
                <md-table-head>Description</md-table-head>
              </md-table-row>
            </md-table-header>

            <md-table-body>
              <md-table-row>
                <md-table-cell>md-fixed</md-table-cell>
                <md-table-cell><code>Boolean</code></md-table-cell>
                <md-table-cell>Make the tabs navigation fixed and elastic filling the whole space. <br>Default: <code>false</code></md-table-cell>
              </md-table-row>

              <md-table-row>
                <md-table-cell>md-centered</md-table-cell>
                <md-table-cell><code>Boolean</code></md-table-cell>
                <md-table-cell>Align the tabs navigation to the center. <br>Default: <code>false</code></md-table-cell>
              </md-table-row>

              <md-table-row>
                <md-table-cell>md-right</md-table-cell>
                <md-table-cell><code>Boolean</code></md-table-cell>
                <md-table-cell>Align the tabs navigation to the right. <br>Default: <code>false</code></md-table-cell>
              </md-table-row>

              <md-table-row>
                <md-table-cell>md-dynamic-height</md-table-cell>
                <md-table-cell><code>Boolean</code></md-table-cell>
                <md-table-cell>Make the tab content to be resized based on the contents. <br>Default: <code>true</code></md-table-cell>
              </md-table-row>

              <md-table-row>
                <md-table-cell>md-elevation</md-table-cell>
                <md-table-cell><code>Number</code></md-table-cell>
                <md-table-cell>Add a shadow on the navigation with an whiteframe. <br>Default: <code>0</code></md-table-cell>
              </md-table-row>

              <md-table-row>
                <md-table-cell>md-navigation</md-table-cell>
                <md-table-cell><code>Boolean</code></md-table-cell>
                <md-table-cell>Display the navigation arrows for horizontal scroll. <br>Default: <code>true</code></md-table-cell>
              </md-table-row>
            </md-table-body>
          </md-table>

          <md-table slot="slots">
            <md-table-header>
              <md-table-row>
                <md-table-head>Name</md-table-head>
                <md-table-head>Description</md-table-head>
              </md-table-row>
            </md-table-header>

            <md-table-body>
              <md-table-row>
                <md-table-cell>header-item</md-table-cell>
                <md-table-cell>Change the template of the header item. Optional.</md-table-cell>
              </md-table-row>
            </md-table-body>
          </md-table>

          <md-table slot="events">
            <md-table-header>
              <md-table-row>
                <md-table-head>Name</md-table-head>
                <md-table-head>Value</md-table-head>
                <md-table-head>Description</md-table-head>
              </md-table-row>
            </md-table-header>

            <md-table-body>
              <md-table-row>
                <md-table-cell>change</md-table-cell>
                <md-table-cell>Receive the tab index</md-table-cell>
                <md-table-cell>Triggered when a tab is activated.</md-table-cell>
              </md-table-row>
            </md-table-body>
          </md-table>
        </api-table>

        <api-table name="md-tab">
          <p>You should wrap the <code>&lt;md-tab&gt;</code> in a <code>&lt;md-tabs&gt;</code> as a direct parent.</p>
          <md-table slot="properties">
            <md-table-header>
              <md-table-row>
                <md-table-head>Name</md-table-head>
                <md-table-head>Type</md-table-head>
                <md-table-head>Description</md-table-head>
              </md-table-row>
            </md-table-header>

            <md-table-body>
              <md-table-row>
                <md-table-cell>id</md-table-cell>
                <md-table-cell><code>String</code></md-table-cell>
                <md-table-cell>Unique id to each tab</md-table-cell>
              </md-table-row>

              <md-table-row>
                <md-table-cell>md-label</md-table-cell>
                <md-table-cell><code>String</code></md-table-cell>
                <md-table-cell>The tab text</md-table-cell>
              </md-table-row>

              <md-table-row>
                <md-table-cell>md-options</md-table-cell>
                <md-table-cell><code>any</code></md-table-cell>
                <md-table-cell>Any additional options (which can be used in <code>header-item</code> slot of <code>md-tabs</code>)</md-table-cell>
              </md-table-row>

              <md-table-row>
                <md-table-cell>md-icon</md-table-cell>
                <md-table-cell><code>String</code></md-table-cell>
                <md-table-cell>Icon name on the <a href="https://material.io/icons/" target="_blank" rel="noopener">Material Icons</a> docs.</md-table-cell>
              </md-table-row>

              <md-table-row>
                <md-table-cell>md-iconset</md-table-cell>
                <md-table-cell><code>String</code></md-table-cell>
                <md-table-cell>Allows use of icons from another iconset. <br>Example: <code>md-iconset="fa fa-pencil"</code> for font awesome. </md-table-cell>
              </md-table-row>

              <md-table-row>
                <md-table-cell>md-icon-src</md-table-cell>
                <md-table-cell><code>String</code></md-table-cell>
                <md-table-cell>Path to a custom PNG/SVG image.</md-table-cell>
              </md-table-row>

              <md-table-row>
                <md-table-cell>md-active</md-table-cell>
                <md-table-cell><code>Boolean</code></md-table-cell>
                <md-table-cell>Activate the tab. <br>Default: <code>false</code></md-table-cell>
              </md-table-row>

              <md-table-row>
                <md-table-cell>md-disabled</md-table-cell>
                <md-table-cell><code>Boolean</code></md-table-cell>
                <md-table-cell>Disable the tab and prevent its actions. <br>Default: <code>false</code></md-table-cell>
              </md-table-row>

              <md-table-row>
                <md-table-cell>md-tooltip</md-table-cell>
                <md-table-cell><code>String</code></md-table-cell>
                <md-table-cell>Add a tooltip on the tab header. Optional.</md-table-cell>
              </md-table-row>

              <md-table-row>
                <md-table-cell>md-tooltip-delay</md-table-cell>
                <md-table-cell><code>String</code></md-table-cell>
                <md-table-cell>Delay of the tab header tooltip. <br>Default: <code>0</code></md-table-cell>
              </md-table-row>

              <md-table-row>
                <md-table-cell>md-tooltip-direction</md-table-cell>
                <md-table-cell><code>String</code></md-table-cell>
                <md-table-cell>Direction of the tab header tooltip. <br>Default: <code>bottom</code></md-table-cell>
              </md-table-row>
            </md-table-body>
          </md-table>
        </api-table>
      </div>

      <div slot="example">
        <example-box card-title="Default">
          <div slot="demo">
            <md-tabs :md-dynamic-height="false">
              <md-tab id="movies" md-label="Movies">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.</p>
              </md-tab>

              <md-tab id="music" md-label="Music">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.</p>
              </md-tab>

              <md-tab id="books" md-label="Books">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.</p>
              </md-tab>

              <md-tab id="pictures" md-label="Pictures">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.</p>
              </md-tab>

              <md-tab id="playlists" md-label="Playlists">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.</p>
              </md-tab>

              <md-tab id="albums" md-label="Albums">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.</p>
              </md-tab>

              <md-tab id="settings" md-label="Settings">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.</p>
              </md-tab>

              <md-tab id="account" md-label="Account">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.</p>
              </md-tab>
            </md-tabs>
          </div>

          <div slot="code">
            <code-block lang="xml">
              &lt;md-tabs&gt;
                &lt;md-tab id=&quot;movies&quot; md-label=&quot;Movies&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.&lt;/p&gt;
                &lt;/md-tab&gt;

                &lt;md-tab id=&quot;music&quot; md-label=&quot;Music&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.&lt;/p&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.&lt;/p&gt;
                &lt;/md-tab&gt;

                &lt;md-tab id=&quot;books&quot; md-label=&quot;Books&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.&lt;/p&gt;
                &lt;/md-tab&gt;

                &lt;md-tab id=&quot;pictures&quot; md-label=&quot;Pictures&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.&lt;/p&gt;
                &lt;/md-tab&gt;

                &lt;md-tab id=&quot;playlists&quot; md-label=&quot;Playlists&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.&lt;/p&gt;
                &lt;/md-tab&gt;

                &lt;md-tab id=&quot;albums&quot; md-label=&quot;Albums&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.&lt;/p&gt;
                &lt;/md-tab&gt;

                &lt;md-tab id=&quot;settings&quot; md-label=&quot;Settings&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.&lt;/p&gt;
                &lt;/md-tab&gt;

                &lt;md-tab id=&quot;account&quot; md-label=&quot;Account&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.&lt;/p&gt;
                &lt;/md-tab&gt;
              &lt;/md-tabs&gt;
            </code-block>
          </div>
        </example-box>

        <example-box card-title="Fixed">
          <div slot="demo">
            <md-tabs :md-dynamic-height="false" md-fixed class="md-accent">
              <md-tab id="movies" md-label="Movies">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.</p>
              </md-tab>

              <md-tab id="music" md-label="Music">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.</p>
              </md-tab>

              <md-tab id="books" md-label="Books">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.</p>
              </md-tab>

              <md-tab id="pictures" md-label="Pictures">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.</p>
              </md-tab>
            </md-tabs>
          </div>

          <div slot="code">
            <code-block lang="xml">
              &lt;md-tabs md-fixed&gt;
                &lt;md-tab id=&quot;movies&quot; md-label=&quot;Movies&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.&lt;/p&gt;
                &lt;/md-tab&gt;

                &lt;md-tab id=&quot;music&quot; md-label=&quot;Music&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.&lt;/p&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.&lt;/p&gt;
                &lt;/md-tab&gt;

                &lt;md-tab id=&quot;books&quot; md-label=&quot;Books&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.&lt;/p&gt;
                &lt;/md-tab&gt;

                &lt;md-tab id=&quot;pictures&quot; md-label=&quot;Pictures&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.&lt;/p&gt;
                &lt;/md-tab&gt;
              &lt;/md-tabs&gt;
            </code-block>
          </div>
        </example-box>

        <example-box card-title="Centered with Text and Icon">
          <div slot="demo">
            <md-tabs :md-dynamic-height="false" md-centered class="md-warn">
              <md-tab md-label="Movies" md-icon="ondemand_video">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.</p>
              </md-tab>

              <md-tab md-label="Music" md-icon="music_note">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.</p>
              </md-tab>

              <md-tab md-label="Books" md-icon="books">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.</p>
              </md-tab>

              <md-tab md-label="Pictures" md-icon="photo">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.</p>
              </md-tab>
            </md-tabs>
          </div>

          <div slot="code">
            <code-block lang="xml">
              &lt;md-tabs md-centered&gt;
                &lt;md-tab md-label=&quot;Movies&quot; md-icon=&quot;ondemand_video&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.&lt;/p&gt;
                &lt;/md-tab&gt;

                &lt;md-tab md-label=&quot;Music&quot; md-icon=&quot;music_note&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.&lt;/p&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.&lt;/p&gt;
                &lt;/md-tab&gt;

                &lt;md-tab md-label=&quot;Books&quot; md-icon=&quot;books&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.&lt;/p&gt;
                &lt;/md-tab&gt;

                &lt;md-tab md-label=&quot;Pictures&quot; md-icon=&quot;photo&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.&lt;/p&gt;
                &lt;/md-tab&gt;
              &lt;/md-tabs&gt;
            </code-block>
          </div>
        </example-box>

        <example-box card-title="Aligned to the right with only icons">
          <div slot="demo">
            <md-tabs :md-dynamic-height="false" md-right class="md-transparent">
              <md-tab md-icon="phone">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.</p>
              </md-tab>

              <md-tab md-icon="favorite">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.</p>
              </md-tab>

              <md-tab md-icon="near_me">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.</p>
              </md-tab>
            </md-tabs>
          </div>

          <div slot="code">
            <code-block lang="xml">
              &lt;md-tabs md-right&gt;
                &lt;md-tab md-icon=&quot;phone&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.&lt;/p&gt;
                &lt;/md-tab&gt;

                &lt;md-tab md-icon=&quot;favorite&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.&lt;/p&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.&lt;/p&gt;
                &lt;/md-tab&gt;

                &lt;md-tab md-icon=&quot;near_me&quot;&gt;
                  &lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.&lt;/p&gt;
                &lt;/md-tab&gt;
              &lt;/md-tabs&gt;
            </code-block>
          </div>
        </example-box>

        <example-box card-title="Header item templating">
          <div slot="demo">
            <md-tabs class="md-transparent">
              <template slot="header-item" scope="props">
                <md-icon v-if="props.header.icon">{{ props.header.icon }}</md-icon>
                <template v-if="props.header.options && props.header.options.new_badge">
                  <span v-if="props.header.label" class="label-with-new-badge">
                    {{ props.header.label }}
                    <span class="new-badge">{{props.header.options.new_badge}}</span>
                  </span>
                </template>
                <template v-else>
                  <span v-if="props.header.label">{{ props.header.label }}</span>
                </template>
              </template>
              <md-tab md-icon="phone" md-label="Phone">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.</p>
              </md-tab>

              <md-tab md-icon="favorite" md-label="Favorite" :md-options="{new_badge: 3}">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.</p>
              </md-tab>

              <md-tab md-icon="near_me" md-label="Near me" :md-options="{new_badge: 1}">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.</p>
              </md-tab>
            </md-tabs>
          </div>

          <div slot="code">
            <code-block lang="xml">
              &#x3C;md-tabs class=&#x22;md-transparent&#x22;&#x3E;
                &#x3C;template slot=&#x22;header-item&#x22; scope=&#x22;props&#x22;&#x3E;
                  &#x3C;md-icon v-if=&#x22;props.header.icon&#x22;&#x3E;{{ '\x7b\x7b' }} props.header.icon {{ '\x7d\x7d' }}&#x3C;/md-icon&#x3E;
                  &#x3C;template v-if=&#x22;props.header.options &#x26;&#x26; props.header.options.new_badge&#x22;&#x3E;
                    &#x3C;span v-if=&#x22;props.header.label&#x22; class=&#x22;label-with-new-badge&#x22;&#x3E;
                      {{ '\x7b\x7b' }} props.header.label {{ '\x7d\x7d' }}
                      &#x3C;span class=&#x22;new-badge&#x22;&#x3E;{{ '\x7b\x7b' }} props.header.options.new_badge {{ '\x7d\x7d' }}&#x3C;/span&#x3E;
                    &#x3C;/span&#x3E;
                  &#x3C;/template&#x3E;
                  &#x3C;template v-else&#x3E;
                    &#x3C;span v-if=&#x22;props.header.label&#x22;&#x3E;{{ '\x7b\x7b' }} props.header.label {{ '\x7d\x7d' }}&#x3C;/span&#x3E;
                  &#x3C;/template&#x3E;
                &#x3C;/template&#x3E;
                &#x3C;md-tab md-icon=&#x22;phone&#x22; md-label=&#x22;Phone&#x22;&#x3E;
                  &#x3C;p&#x3E;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.&#x3C;/p&#x3E;
                &#x3C;/md-tab&#x3E;

                &#x3C;md-tab md-icon=&#x22;favorite&#x22; md-label=&#x22;Favorite&#x22; :md-options=&#x22;&#x7B;new_badge: 3&#x7D;&#x22;&#x3E;
                  &#x3C;p&#x3E;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.&#x3C;/p&#x3E;
                  &#x3C;p&#x3E;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas amet cum vitae, omnis! Illum quas voluptatem, expedita iste, dicta ipsum ea veniam dolore in, quod saepe reiciendis nihil.&#x3C;/p&#x3E;
                &#x3C;/md-tab&#x3E;

                &#x3C;md-tab md-icon=&#x22;near_me&#x22; md-label=&#x22;Near me&#x22; :md-options=&#x22;&#x7B;new_badge: 1&#x7D;&#x22;&#x3E;
                  &#x3C;p&#x3E;Lorem ipsum dolor sit amet, consectetur adipisicing elit. Deserunt dolorum quas.&#x3C;/p&#x3E;
                &#x3C;/md-tab&#x3E;
              &#x3C;/md-tabs&#x3E;
            </code-block>
          </div>
        </example-box>
      </div>
    </docs-component>
  </page-content>
</template>

<style>
  .label-with-new-badge {
    font-weight: bolder;
  }
  .new-badge {
    background-color: red;
    color: white;
    padding: 3px;
    border-radius: 3px;
  }
</style>
