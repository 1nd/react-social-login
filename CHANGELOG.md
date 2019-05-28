# Change Log

## v4.0.0 [28 May 2019]

### Breaking Changes
 * Change package name to `@1nd/react-social-login` because this is fork.
 * Do not support React before v16.1.0.
 * Remove `whatwg-fetch` polyfill. User can polyfill `fetch` themselves if they need to do it.
 * The public API should stay backward-compatible with `react-social-login` `^3.0.0` so public API does not contain breaking change.

### Other Changes
 * Facebook SDK uses Graph API version 3.3.
 * Move `react` and `react-dom` to `devDependencies` to make sure React version used by `react-social-login` is the same with React version used by `react-social-login` user. Also to prevent error when two different React versions run together.
 * Remove `prop-types` from dependencies because we don't support React older than v16.1.0.
 * Update dependencies: `bluebird`.

Notes: `bluebird` is not removed because `react-social-login` uses Promise cancellation which is not provided by native Promise but provided by Bluebird.

## v3.4.3 [23 December 2018]
Pull Request: [#112](https://github.com/deepakaggarwal7/react-social-login/pull/112).
Changes:
 * Github ID now avilable (Thanks to [MuhamadOmr](https://github.com/deepakaggarwal7/)

## v3.4.2 [26 December 2017]
Fix SSR, refs and update build.
Changes:
 * Fixes url parser when window is undefined (SSR fix)
 * Don’t use refs on stateless components
 * Update build system (`babel-preset-env`, updated dependencies, lighter npm package)

## v3.4.1 [08 November 2017]
Fix logout issues, adds SSR support and fixes.
Changes:
 * Fix unknown prop `triggerLogout` forwarded to wrapped component
 * Server-side rendering support
 * Small fixes
 * Update README to explain how logout is implemented in demo

## v3.4.0 [22 October 2017]
Fix logout issues, expose wrapped component ref and fixes.
Changes:
 * Fix logout issue with Amazon
 * Don’t throw error on Instagram logout (like fake SDK load doesn’t throw)
 * Expose wrapped component ref ([react know issue](https://github.com/facebook/react/issues/4213))
 * Small fixes

## v3.3.0 [22 October 2017]
Logout, custom scopes and fixes.
Changes:
 * Add publicProfileURL for LinkedIn
 * Add logout support
 * Fix wrong GitHub id
 * Add custom scope support (all but LinkedIn)
 * Update documentation

## v3.2.1 [06 October 2017]
React 16, better build, update dep, additions and fixes.
Changes:
 * Update React to v16
 * Update all dependencies to latest stable versions
 * Optimize webpack build
 * Return full googleAuthResponse
 * Preserve redirect url query string and hash
 * Cancel loading on componentWillUnmount
 * Various fixes

## v3.2.0 [14 September 2017]
 * Custom Google scopes
 * Multiple Google buttons
 * GitHub doc

## v3.1.0 [01 August 2017]
Pull Request: [#20](https://github.com/deepakaggarwal7/react-social-login/pull/20).
Changes:
 * Amazon
 * https

## v3.0.0 [30 July 2017]
Pull Request: [#19](https://github.com/deepakaggarwal7/react-social-login/pull/19).
Changes:
 * Rewrote as HOC
 * Instagram
 * GitHub
 * Auto login
 * Better error handling
 * Various fixes

## v2.0.1 [24 June 2017]
Pull Request: [#15](https://github.com/deepakaggarwal7/react-social-login/pull/15).
Changes:
 * Facebook error
 * code styling
 * unnecessary console logs
 * pre-commit lint

## v2.0.0 [26 Feb 2017]
 * Use small case for providers
 * Linkedin support added along with previous google and facebook
 * A lot of refactoring done
 * Uses Webpack 2.x

__Huge  Thanks to  Nicolas Goudry for his generous contribution __