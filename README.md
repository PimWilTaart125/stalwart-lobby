# Stalwart Lobby

A custom web app for Stalwart, designed to act as a bridge between the Stalwart WebUI and Bulwark Webmail Lite.

## Installation

### 1. Create the application

In the Stalwart WebUI, go to:

**Settings → Web Applications → Create Application**

Use these settings:

| Setting              | Value                                                                               |
| -------------------- | ----------------------------------------------------------------------------------- |
| **Resource URL**     | `https://github.com/PimWilTaart125/stalwart-lobby/releases/download/V2.1/index.zip` |
| **URL Prefix**       | `/lobby`                                                                            |
| **Description**      | `Stalwart Lobby`                                                                    |                                                                                   |
| **Update Frequency** | Default                                                                             |

You can replace `/lobby` with another prefix such as `/home`.

Click **Save** when finished.

### 2. Update the application

After installing, go to:

**Management → Actions → Update Applications**

Click **Update Applications** and wait for the update to finish.

## Redirect `/` to the Lobby

To make the Lobby the first page users see:

1. Go to **Settings → Network → HTTP → General**.
2. Find **Redirect root**.
3. Set it to your application prefix:

```URL
/lobby
```

4. Save the settings.
5. Restart Stalwart.

Now visiting:

```URL
https://your-domain.com/
```

will redirect users to:

```URL
https://your-domain.com/lobby
```

## Updating

When a new version is released, update the **Resource URL** if necessary and run:

**Management → Actions → Update Applications**

That's it! 🎉
