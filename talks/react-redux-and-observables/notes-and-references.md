# React with Redux and Redux-observable

## Notes

```js
export const loadSites = EpicBuilder
  .ofType(types.LOAD_SITES)
  .callApi('Site', 'fetch')
  .mapToSuccess(types.SITES_LOADED)
  .mapToFailure(types.SITES_LOADING_ERROR)
  .create();

export const loadVariables = EpicBuilder
  .ofType(types.LOAD_VARIABLES)
  .callApi('Variable', 'fetch')
  .mapToSuccess(types.VARIABLES_LOADED)
  .mapToFailure(types.VARIABLES_LOADING_ERROR)
  .create();

export const saveProject = EpicBuilder
  .ofType(types.SAVE_PROJECT)
  .callApi('Project', 'merge')
  .mapToSuccess(types.LOAD_PROJECTS)
  .mapToFailure(types.PROJECT_SAVING_ERROR)
  .create();
```


https://fr.slideshare.net/jayphelps/rxjs-redux-react-amazing
https://jrsinclair.com/articles/2018/react-redux-javascript-architecture/