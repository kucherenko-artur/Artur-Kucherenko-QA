# API Test Cases

## API-TC-001 — GET /items returns 200 and list

**Steps:** Send GET /items

**Expected:** 200 OK, JSON list

## API-TC-002 — POST /items valid body returns 201

**Steps:** Send POST with valid body

**Expected:** 201 Created, new id

## API-TC-003 — PUT /items/{id} updates returns 200

**Steps:** PUT existing id

**Expected:** 200 OK, updated fields

## API-TC-004 — DELETE /items/{id} returns 204

**Steps:** DELETE existing id

**Expected:** 204 No Content

## API-TC-005 — POST /items invalid body returns 400

**Steps:** POST invalid schema

**Expected:** 400 Bad Request with error details

## API-TC-006 — GET /items/{id} not found returns 404

**Steps:** GET nonexistent id

**Expected:** 404 Not Found
