<p align="center">
    <img src="https://user-images.githubusercontent.com/6702424/109387840-eba11f80-7903-11eb-9050-db1dad883f78.png">  
</p>
<p align="center">
    <i>🔏 Create Keycloak themes using React 🔏</i>
    <br>
    <br>
    <a href="https://github.com/garronej/keycloakify/actions">
      <img src="https://github.com/garronej/keycloakify/workflows/ci/badge.svg?branch=main">
    </a>
    <a href="https://www.npmjs.com/package/keycloakify">
      <img src="https://img.shields.io/npm/dm/keycloakify">
    </a>
    <a href="https://github.com/garronej/keycloakify/blob/main/LICENSE">
      <img src="https://img.shields.io/npm/l/keycloakify">
    </a>
    <a href="https://github.com/InseeFrLab/keycloakify/blob/729503fe31a155a823f46dd66ad4ff34ca274e0a/tsconfig.json#L14">
        <img src="https://camo.githubusercontent.com/0f9fcc0ac1b8617ad4989364f60f78b2d6b32985ad6a508f215f14d8f897b8d3/68747470733a2f2f62616467656e2e6e65742f62616467652f547970655363726970742f7374726963742532302546302539462539322541412f626c7565">
    </a>
    <a href="https://github.com/thomasdarimont/awesome-keycloak">
        <img src="https://awesome.re/mentioned-badge.svg"/>
    </a>
    <p align="center">
        <a href="https://www.keycloakify.dev">Home</a>
        -
        <a href="https://docs.keycloakify.dev">Documentation</a>
        -
        <a href="https://storybook.keycloakify.dev/storybook">Storybook</a>
        -
        <a href="https://github.com/codegouvfr/keycloakify-starter">Starter project</a>
    </p>
</p>

<p align="center">
    <i>Ultimately this build tool generates a Keycloak theme <a href="https://www.keycloakify.dev">Learn more</a></i>
    <img src="https://user-images.githubusercontent.com/6702424/110260457-a1c3d380-7fac-11eb-853a-80459b65626b.png">
</p>

> 🗣 V6 have been released 🎉  
> [It features major improvements](https://github.com/InseeFrLab/keycloakify#600).  
> Checkout [the migration guide](https://docs.keycloakify.dev/v5-to-v6).

# Changelog highlights

## 7.0 🍾

-   Account theme support 🚀
-   It's much easier to customize pages at the CSS level, you can now see in the browser dev tool the customizable classes.
-   New interactive CLI tool `npx eject-keycloak-page`, that enables to select the page you want to customize at the component level.
-   There is [a Storybook](https://storybook.keycloakify.dev)
-   [Remember me is fixed](https://github.com/InseeFrLab/keycloakify/pull/272)

## 6.13

-   Build work behind corporate proxies, [see issue](https://github.com/InseeFrLab/keycloakify/issues/257).

## 6.12

Massive improvement in the developer experience:

-   There is now only one starter repo: https://github.com/codegouvfr/keycloakify-starter
-   A lot of comments have been added in the code of the starter to make it easier to get started.
-   The doc has been updated: https://docs.keycloakify.dev
-   A lot of improvements in the type system.

## 6.11.4

-   You no longer need to have Maven installed to build the theme. Thanks to @lordvlad, [see PR](https://github.com/InseeFrLab/keycloakify/pull/239).
-   Feature new build options: [`bundler`](https://docs.keycloakify.dev/build-options#keycloakify.bundler), [`groupId`](https://docs.keycloakify.dev/build-options#keycloakify.groupid), [`artifactId`](https://docs.keycloakify.dev/build-options#keycloakify.artifactid), [`version`](https://docs.keycloakify.dev/build-options#version).  
    Theses options can be user to customize the output name of the .jar. You can use environnement variables to overrides the values read in the package.json. Thanks to @lordvlad.

## 6.10.0

-   Widows compat (thanks to @lordvlad, [see PR](https://github.com/InseeFrLab/keycloakify/pull/226)). WSL is no longer required 🎉

## 6.8.4

-   `@emotion/react` is no longer a peer dependency of Keycloakify.

## 6.8.0

-   It is now possible to pass a custom `<Template />` component as a prop to `<KcApp />` and every
    individual page (`<Login />`, `<RegisterUserProfile />`, ...) it enables to customize only the header and footer for
    example without having to switch to a full-component level customization. [See issue](https://github.com/InseeFrLab/keycloakify/issues/191).

## 6.7.0

-   Add support for `webauthn-authenticate.ftl` thanks to [@mstrodl](https://github.com/Mstrodl)'s hacktoberfest [PR](https://github.com/InseeFrLab/keycloakify/pull/185).

## 6.6.0

-   Add support for `login-password.ftl` thanks to [@mstrodl](https://github.com/Mstrodl)'s hacktoberfest [PR](https://github.com/InseeFrLab/keycloakify/pull/184).

## 6.5.0

-   Add support for `login-username.ftl` thanks to [@mstrodl](https://github.com/Mstrodl)'s hacktoberfest [PR](https://github.com/InseeFrLab/keycloakify/pull/183).

## 6.4.0

-   You can now optionally pass a `doFetchDefaultThemeResources: boolean` prop to every page component and the default `<KcApp />`
    This enables you to prevent the default CSS and JS that comes with the builtin Keycloak theme to be downloaded.  
    You'll get [a black slate](https://user-images.githubusercontent.com/6702424/192619083-4baa5df4-4a21-4ec7-8e28-d200d1208299.png).

## 6.0.0

-   Bundle size drastically reduced, locals and component dynamically loaded.
-   First print much quicker, use of React.lazy() everywhere.
-   Real i18n API.
-   Actual documentation for build options.

Checkout [the migration guide](https://docs.keycloakify.dev/v5-to-v6)

## 5.8.0

-   [React.lazy()](https://reactjs.org/docs/code-splitting.html#reactlazy) support 🎉. [#141](https://github.com/InseeFrLab/keycloakify/issues/141)

## 5.7.0

-   Feat `logout-confirm.ftl`. [PR](https://github.com/InseeFrLab/keycloakify/pull/120)

## 5.6.4

Fix `login-verify-email.ftl` page. [Before](https://user-images.githubusercontent.com/6702424/177436014-0bad22c4-5bfb-45bb-8fc9-dad65143cd0c.png) - [After](https://user-images.githubusercontent.com/6702424/177435797-ec5d7db3-84cf-49cb-8efc-3427a81f744e.png)

## v5.6.0

Add support for `login-config-totp.ftl` page [#127](https://github.com/InseeFrLab/keycloakify/pull/127).

## v5.3.0

Rename `keycloak_theme_email` to `keycloak_email`.  
If you already had a `keycloak_theme_email` you should rename it `keycloak_email`.

## v5.0.0

[Migration guide](https://github.com/garronej/keycloakify-demo-app/blob/a5b6a50f24bc25e082931f5ad9ebf47492acd12a/src/index.tsx#L46-L63)  
New i18n system.  
Import of terms and services have changed. [See example](https://github.com/garronej/keycloakify-demo-app/blob/a5b6a50f24bc25e082931f5ad9ebf47492acd12a/src/index.tsx#L46-L63).

## v4.10.0

Add `login-idp-link-email.ftl` page [See PR](https://github.com/InseeFrLab/keycloakify/pull/92).

## v4.8.0

[Email template customization.](#email-template-customization)

## v4.7.4

**M1 Mac** support (for testing locally with a dockerized Keycloak).

## v4.7.2

> WARNING: This is broken.  
> Testing with local Keycloak container working with M1 Mac. Thanks to [@eduardosanzb](https://github.com/InseeFrLab/keycloakify/issues/43#issuecomment-975699658).  
> Be aware: When running M1s you are testing with Keycloak v15 else the local container spun will be a Keycloak v16.1.0.

## v4.7.0

Register with user profile enabled: Out of the box `options` validator support.  
[Example](https://user-images.githubusercontent.com/6702424/158911163-81e6bbe8-feb0-4dc8-abff-de199d7a678e.mov)

## v4.6.0

`tss-react` and `powerhooks` are no longer peer dependencies of `keycloakify`.
After updating Keycloakify you can remove `tss-react` and `powerhooks` from your dependencies if you don't use them explicitly.

## v4.5.3

There is a new recommended way to setup highly customized theme. See [here](https://github.com/garronej/keycloakify-demo-app/blob/look_and_feel/src/KcApp/KcApp.tsx).  
Unlike with [the previous recommended method](https://github.com/garronej/keycloakify-demo-app/blob/a51660578bea15fb3e506b8a2b78e1056c6d68bb/src/KcApp/KcApp.tsx),
with this new method your theme wont break on minor Keycloakify update.

## v4.3.0

Feature [`login-update-password.ftl`](https://user-images.githubusercontent.com/6702424/147517600-6191cf72-93dd-437b-a35c-47180142063e.png).  
Every time a page is added it's a breaking change for non CSS-only theme.  
Change [this](https://github.com/garronej/keycloakify-demo-app/blob/df664c13c77ce3c53ac7df0622d94d04e76d3f9f/src/KcApp/KcApp.tsx#L17) and [this](https://github.com/garronej/keycloakify-demo-app/blob/df664c13c77ce3c53ac7df0622d94d04e76d3f9f/src/KcApp/KcApp.tsx#L37) to update.

## v4

-   Out of the box [frontend form validation](#user-profile-and-frontend-form-validation) 🥳
-   Improvements (and breaking changes in `import { useKcMessage } from "keycloakify"`.

## v3

No breaking changes except that `@emotion/react`, [`tss-react`](https://www.npmjs.com/package/tss-react) and [`powerhooks`](https://www.npmjs.com/package/powerhooks) are now `peerDependencies` instead of being just dependencies.  
It's important to avoid problem when using `keycloakify` alongside [`mui`](https://mui.com) and
[when passing params from the app to the login page](https://github.com/InseeFrLab/keycloakify#implement-context-persistence-optional).

## v2.5

-   Feature [Use advanced message](https://github.com/InseeFrLab/keycloakify/blob/59f106bf9e210b63b190826da2bf5f75fc8b7644/src/lib/i18n/useKcMessage.tsx#L53-L66)
    and [`messagesPerFields`](https://github.com/InseeFrLab/keycloakify/blob/59f106bf9e210b63b190826da2bf5f75fc8b7644/src/lib/getKcContext/KcContextBase.ts#L70-L75) (implementation [here](https://github.com/InseeFrLab/keycloakify/blob/59f106bf9e210b63b190826da2bf5f75fc8b7644/src/bin/build-keycloak-theme/generateFtl/common.ftl#L130-L189))
-   Test container now uses Keycloak version `15.0.2`.

## v2

-   It's now possible to implement custom `.ftl` pages.
-   Support for Keycloak plugins that introduce non standard ftl values.
    (Like for example [this plugin](https://github.com/micedre/keycloak-mail-whitelisting) that define `authorizedMailDomains` in `register.ftl`).
