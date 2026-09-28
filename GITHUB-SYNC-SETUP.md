# GitHub-only Admin and Viewer setup

No external database is required.

## Dashboard links

- Viewer: `https://aboodimtiaz7.github.io/aditi-workforce-intelligence/`
- Admin: `https://aboodimtiaz7.github.io/aditi-workforce-intelligence/?view=admin`

## Create the restricted admin token

1. In GitHub, open **Settings → Developer settings → Personal access tokens → Fine-grained tokens**.
2. Select **Generate new token**.
3. Give it a short expiry and select only the `aditi-workforce-intelligence` repository.
4. Under **Repository permissions**, give **Contents** read and write access. Leave other permissions unchanged.
5. Create and copy the token. Do not add it to any repository file.

## Use the Admin view

1. Open the Admin link and select **Connect GitHub**.
2. Paste the restricted token. It is kept only in the current browser tab session.
3. Select **Edit dashboard** and make changes.
4. Changes save in the browser automatically and survive refresh.
5. After editing pauses, the Admin view automatically updates `dashboard-data.json` in GitHub.
6. GitHub Pages republishes the change. Viewer pages check for updated data every 15 seconds.

The manual **Publish updates** button remains available as a backup.
