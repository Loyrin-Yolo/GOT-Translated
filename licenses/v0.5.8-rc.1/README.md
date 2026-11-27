# Third-party licensing — GOT TRANSLATED v0.5.8 RC1

**Inventory and reference materials; review incomplete.** This directory is not a license grant for GOT TRANSLATED, Arknights, or the complete binary distribution. Do not interpret a listed upstream license as proof that every packaged binary is covered by it.

- `THIRD_PARTY_NOTICE.txt` and `LICENSE_AUDIT_RU.txt`: existing preliminary notices and outstanding review.
- `runtime_inventory.json`: SHA256, size and relative path of every runtime member.
- `reference/`: reference license texts. XUnity v5.6.1 MIT text transcribed from the tagged upstream LICENSE; LGPL-2.1 is the standard license text, not proof of provenance of a specific DLL.
- `upstream/`: exact-ref license/notice documents collected when available (no fallback to latest/master).
- `build_environment/`: available notices for the actual developer Python/build environment (not proof that every dependency of the frozen executable is covered).
- `collection_status.json`: provenance and missing-document checklist.
- `reviewed/` (optional): additional independently reviewed redistribution documents, source materials and notices supplied by the maintainer. Only put public materials here.

## Upstream references

| Component | Candidate version/source | Notes |
|---|---|---|
| BepInEx | [6.0.0-be.697+5362580](https://builds.bepinex.dev/projects/bepinex_be) / [source](https://github.com/BepInEx/BepInEx/tree/5362580) | LGPL-2.1; match binary and provide corresponding source and applicable notices. |
| UnityDoorstop | [4.3.0](https://github.com/NeighTools/UnityDoorstop/releases) | Doorstop 4 upstream identifies LGPL-2.1; exact-tag license and binary correspondence must be checked. |
| XUnity.AutoTranslator | [v5.6.1 LICENSE](https://github.com/bbepis/XUnity.AutoTranslator/blob/v5.6.1/LICENSE) | MIT; verify actual binaries, ResourceRedirector, ExIni and dependencies. |
| .NET | 6.0.7, `0ec02c8c96e2eda06dc5b5edfdbdba0f36415082` from runtime .version | [runtime](https://github.com/dotnet/runtime), [BepInEx fork](https://github.com/BepInEx/dotnet-runtime), [licensing info](https://github.com/dotnet/core/blob/main/license-information.md). Match actual binary distribution including third-party notices and fork changes. |
| LocalizationToolkit | user-supplied v2.0.0; upstream identity and redistribution terms pending | Not a separate installed application in this package. Audit provenance of retained components. |

Unresolved: dependency-specific versions and licenses (HarmonyX, MonoMod, Il2CppInterop, Cpp2IL, AsmResolver, AssetRipper, etc.), complete corresponding source where required, frozen runtime notices and actual binary provenance, rights to dictionaries/art and game authorization. No claim of complete legal review. The main repository folder and the user's ZIP both carry these documents; no separate release assets are necessary. The public binary release gate remains independent.
