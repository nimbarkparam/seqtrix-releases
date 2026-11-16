# End User License Agreement

Version 2.0. Last updated 2026-11-05 (5 November 2026); Seqtrix 0.16.0 shows this version as dated 2026-10-13. Applies to the Seqtrix desktop application for Microsoft Windows.

## 1. Who we are and what you are agreeing to

Seqtrix is made and sold by Param Nimbark, a solo founder in Ahmedabad, India (“we”, “us”). This agreement (the “EULA”) is between you and us for the Seqtrix desktop application for Windows, including its templates, updates and documentation (the “Software”).

By ticking the acceptance box in the app, or by installing or using the Software, you agree to this EULA. If you do not agree, do not install or use the Software. You must be 18 or older.

Your account, passes, payments, refunds, the share gallery and the use of seqtrix.com are governed by the [Terms of Service](https://seqtrix.com/terms). What leaves your PC and when is described in the [Privacy Policy](https://seqtrix.com/privacy). Refunds follow the [Refund and Cancellation Policy](https://seqtrix.com/refund-policy). If this EULA and the Terms of Service conflict about the Software itself, this EULA wins; about payments and your account, the Terms of Service win.

## 2. Your licence

We grant you a limited, non-exclusive, non-transferable, revocable licence to install and use the Software on computers that you own or control, for your personal use or the internal use of your business. The Software is licensed, not sold.

The free Starter tier needs no account and no payment. Paid features (Advanced and Pro) unlock for the term of a pass you buy, or under a Pro Lifetime licence if we offer one (section 4). A pass or licence is tied to the account you bought it with. It may be used on more than one computer that you own or control, as long as the account signs in on each one; it may not be shared with other people.

Templates are part of the Software. Which templates you can use depends on your tier. You may change any unlocked template for your own use.

## 3. Tiers, the licence check and what happens when a pass ends

The Software checks your plan on launch and about every 30 minutes. The check sends a hashed identifier for your device and receives a signed entitlement token that unlocks paid features. The token is verified inside the Software. If a check fails, the Software falls back to Starter until a check succeeds. Started without a connection, it keeps the last answer, if that answer is less than 24 hours old, only until its next check.

When a pass ends, paid features stop and the Software returns to Starter on its own. Nothing you made is deleted. Sequences above the Starter limits stay saved and are marked as drafts until you buy again. Encrypted files, vaults and locked items can still be opened with their passwords.

We may change what each tier includes. A change never applies to a pass already bought: you keep what the pass included on the day you paid, until it ends.

## 4. Passes, renewal and Pro Lifetime

- A pass is one payment for a fixed term: 30 days or 365 days. It does not renew by itself, no card is kept on file and there is nothing to cancel. Buy again when it ends.
- Auto-renew is not offered today. If we offer it, it will be a separate, unticked choice at checkout, with the amount and interval shown before you agree, an email before each charge and the option to cancel at any time, as the Terms of Service describe.
- Prices are in US dollars. INR is available if you choose it at checkout. Bank conversion fees are yours.
- Pro Lifetime is not on sale today. If it is offered, “Lifetime” means the life of the product, not your life: Pro features for as long as Seqtrix is sold and supported. If we discontinue Seqtrix, the last released version keeps working within the Starter limits: its Pro features end once we no longer answer the licence check in section 3. Within 12 months of your purchase you may email us for a refund of the Lifetime price less the Pro pass value of the months you held it; after 12 months there is no refund. A Lifetime licence is tied to your account and cannot be transferred.
- Refunds: a full refund within 7 days of purchase if the pass has not been activated in the Software. After activation, only for a verified defect we cannot fix within 7 days of your report, or a Seqtrix-side outage of more than 48 continuous hours. The [Refund and Cancellation Policy](https://seqtrix.com/refund-policy) is the full rule.

## 5. Updates

On launch the Software looks for a newer version and downloads it in the background. You choose when to restart. Each update bundle is signed with our update key and the Software refuses an update whose signature does not verify. By installing the Software you agree to receive updates this way.

Updates may add, change or remove features, change the licence check in section 3 and ask you to accept a new version of this EULA. We try not to remove features without telling you in the in-app changelog first. You may stop using the Software at any time if you do not want an update.

## 6. The installer and code signing

The installer you download from seqtrix.com is not signed with a commercial code-signing certificate. Windows SmartScreen may show a warning the first time you run it. What we do sign is the update bundle (section 5), with our own update key, so an installed copy only accepts updates from us. The Microsoft Store build, where available, is signed by Microsoft as part of Store publishing.

Download the Software only from seqtrix.com, our release page linked from it, or the Microsoft Store. We are not responsible for copies obtained anywhere else.

## 7. Security features, encryption and your data

Your sequences, schedules, settings and vault live on your PC. They leave it only when you turn on cloud sync, publish a share, or switch on crash reports or usage statistics, each of which is off until you choose it. The Privacy Policy has the full list.

- **Encryption** protects files at rest on your disk with AES-256-GCM and a key derived from a password you choose. It does not protect a file while it is open, a copy kept elsewhere, or a file synced or backed up before it was encrypted. We never receive your passwords and cannot recover an encrypted file without the password.
- **The recovery key** (24 words) is shown once when you create it. Keeping it is your responsibility. We keep no copy and cannot recover it, your Master Mode, your vaults or your locked files without it.
- **Secure delete** overwrites a file before deleting it. On SSDs and some other drives the hardware can keep old copies an overwrite never reaches, and copies in backups, shadow copies, cloud sync or other devices are not touched. Treat it as strong cleanup, not a guarantee of removal.
- **Hide, Password Lock and Vault** work as the Software describes them on screen. Basic hide is not encryption. A vault is not a backup.

You are responsible for keeping backups of anything you cannot afford to lose, and for the files, folders and programs you point a security step at.

## 8. Focus Lock and the Panic key

Focus Lock and the Panic key are productivity aids, not security controls, and we do not guarantee that they block anything. Website blocking edits the Windows hosts file after you approve the elevation prompt; browsers using their own DNS-over-HTTPS provider, VPNs, proxies and other devices get around it. App blocking closes the programs you listed. Firm and Hard sessions are designed to resist being ended early, but on the Microsoft Store build Windows can still uninstall Seqtrix during a Hard session and a Store update may pause the watchdog until Seqtrix opens again. The Panic key needs Seqtrix to be running and takes a few seconds to finish.

You choose what a session blocks and for how long, and you are responsible for the consequences of a session you started, including time, missed work and emergency access. Lost time, a blocked site or a session you could not end early is not a defect.

## 9. Sharing and importing sequences

Publishing a sequence puts its title, description, your publisher name and the steps you tick on a public page at seqtrix.com, under the share-gallery terms in the Terms of Service. Step passwords never travel and your folders become placeholders, but typed text and commands you include do travel. Remove anything secret before you publish. You are responsible for what you publish.

An imported sequence runs actions on your PC once you run it: it can open programs, run commands and encrypt, hide or delete files. The Software shows Run Command and Security Lock steps for review before anything is saved, and nothing runs from the review page. Import only from people you trust. We are not responsible for what a sequence written by someone else does on your PC.

## 10. What you may not do

You may not, and may not let anyone else:

- reverse-engineer, decompile, disassemble or otherwise try to derive the source code of the Software, except where the law gives you that right and it cannot be excluded;
- bypass, disable or tamper with the licence check, the entitlement token, the device identifier, the trial, the update signature check or the tier limits;
- copy, modify, rent, lease, sell, sublicense, redistribute or make the Software available to third parties, or share a pass or account;
- remove or hide any copyright, trademark, version or signature notice in the Software or its installer;
- use the Software to break the law, to attack or gain unauthorised access to any system, or to harm anyone, including by sequences you write, import or share;
- use the Software to build a product that competes with Seqtrix.

Tampering with the licence check or the update signature check is a material breach. We may end your licence, suspend your account and keep the fees for the period of the breach.

## 11. Ownership

We and our licensors own the Software and all intellectual property in it. You own the sequences, files and other content you create with it. “Seqtrix” and the Seqtrix logo are our marks; this EULA gives you no right to use them beyond naming the Software.

## 12. Beta and experimental features

Features marked beta, preview or experimental are provided as they are, may be unstable, and may change or disappear without notice.

## 13. No warranty beyond what the law requires

The Software is provided “as is” and “as available”. To the extent the law allows, we give no warranty of any kind, express or implied, including merchantability, fitness for a particular purpose, non-infringement, or that the Software will be error-free, uninterrupted, or will block, protect, encrypt or delete anything in every case. Nothing said by us or in the Software creates a warranty beyond this EULA. Where the law gives you rights that cannot be excluded, including under the Consumer Protection Act, 2019, those rights stand.

## 14. Limit of liability

To the extent the law allows, we are not liable for indirect, incidental, special, consequential or punitive loss, or for lost profits, revenue, data, files you encrypted, deleted or locked, sequences that did not run or ran wrongly, Focus Lock time, or goodwill, however caused, even if we were told it could happen.

Our total liability for everything arising from this EULA or the Software is limited to the amount you paid us for the Software in the 12 months before the claim. If you paid nothing, our total liability is nil. This limit does not apply where the law does not allow it, including for fraud or for liability that consumer law does not let us limit.

## 15. Termination

You may end this EULA at any time by uninstalling the Software. We may end it with immediate effect if you breach section 10, or on 30 days' notice by email if we discontinue the Software (section 4 says what happens to a Lifetime licence). When this EULA ends, your licence ends and you must uninstall the Software. Your local files remain yours. Sections 7, 8, 9, 11, 13, 14 and 17 survive termination.

## 16. Export

The Software contains encryption. You are responsible for complying with the export and sanctions laws that apply to you, and you confirm you are not barred from receiving the Software under the laws of India or of your country.

## 17. Governing law and disputes

This EULA is governed by the laws of India. The courts at Ahmedabad, Gujarat, India have exclusive jurisdiction, except where consumer law lets you file where you live. Before filing anything, email us at help@seqtrix.com and give us 30 days to resolve the matter in good faith.

## 18. Changes to this EULA and the whole agreement

When this EULA changes materially, the version number and date at the top change and the Software asks every install to accept the new version on its next launch. The version shown in the Software's acceptance screen is the version you agreed to. This EULA, the Terms of Service and the Privacy Policy are the whole agreement between you and us about the Software. If any part is unenforceable, the rest stands.

## 19. Contact

Param Nimbark, solo founder, Ahmedabad, India. Email [help@seqtrix.com](mailto:help@seqtrix.com) for questions about this EULA, refunds, data or security. We usually reply within 2 working days.
