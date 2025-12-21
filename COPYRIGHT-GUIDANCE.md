COPYRIGHT & HUMAN AUTHORSHIP GUIDANCE

AI First Exchange (AIFX)

The AI First Exchange (AIFX) recognizes that copyright protection for AI-assisted works generally requires meaningful human creative contribution.
The AIFX standards (AIFM, AIFV, AIFI, AIFP) support documentation of human authorship through structured metadata, declared provenance, and workflow records.

This guidance is informational and does not constitute legal advice.

1. Human Authorship Requirements

An AI-assisted work may be eligible for copyright if a human contributor:

Writes prompts, scripts, or textual instructions

Directs style, tone, structure, pacing, or sequencing

Curates, selects, or rejects generated outputs

Edits, modifies, refines, or enhances AI-generated material

Makes expressive creative decisions that shape the final work

Purely autonomous AI output, without meaningful human creative involvement, is generally not eligible for copyright protection.

2. How AIFX Standards Support Authorship Documentation

AIFX formats support documentation of human involvement by enabling inclusion of:

Creator identity (name, handle, optional contact information)

Human-authored prompts, scripts, or notes

Editing steps and creative decisions

Toolchain and model references

Creation timestamps and declared provenance

This metadata may assist creators, platforms, or rights holders in demonstrating the presence of human creative contribution.

3. Recommended Manifest Fields for Authorship Documentation

Creators MAY include the following optional fields in manifest.json:
```json
"human_authorship_statement": "I affirm that I contributed meaningful creative authorship...",
"human_signature": "Typed name or signature hash",
"creator_email": "email@example.com",
"editorial_notes": "Summary of human creative decisions"
```

These fields are self-declared, optional, and documentation-oriented.

4. Ownership

Copyright ownership belongs to the human author(s) who contributed protectable creative expression.
Works consisting solely of unedited or uncurated machine-generated output may not qualify for copyright protection.

AIFX does not determine ownership or eligibility.

5. Licensing

Creators may include licensing information in legal/license.txt, legal/terms.txt, or equivalent files within an AIFX container.
All distribution and reuse must comply with applicable laws, licenses, and platform policies.

Notes

AIFX does not certify copyright eligibility

AIFX does not verify authorship claims

Legal interpretation is determined by applicable law and downstream authorities
