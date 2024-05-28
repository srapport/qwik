## API Report File for "@builder.io/qwik"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { ClientContainer } from '@builder.io/qwik';
import type { CorePlatform } from '@builder.io/qwik';
import type { _DomContainer } from '@builder.io/qwik';
import type { _ElementVNode } from '@builder.io/qwik';
import type { JSXNode } from '@builder.io/qwik';
import type { JSXOutput } from '@builder.io/qwik';
import type { _QDocument } from '@builder.io/qwik';
import { RenderResult } from '@builder.io/qwik';
import type { _Stringifiable } from '@builder.io/qwik';
import type { _VNode } from '@builder.io/qwik';

// Warning: (ae-forgotten-export) The symbol "MockDocumentOptions" needs to be exported by the entry point index.d.ts
//
// @public
export function createDocument(opts?: MockDocumentOptions): Document;

// @public
export const createDOM: ({ html }?: {
    html?: string;
}) => Promise<{
    render: (jsxElement: JSXOutput) => Promise<RenderResult>;
    screen: HTMLElement;
    userEvent: (queryOrElement: string | Element | keyof HTMLElementTagNameMap | null, eventNameCamel: string | keyof WindowEventMap, eventPayload?: any) => Promise<void>;
}>;

// @public (undocumented)
export function domRender(jsx: JSXOutput, opts?: {
    debug?: boolean;
    oldSSR?: boolean;
}): Promise<{
    document: Document;
    container: ClientContainer;
    vNode: _VNode | null;
    getStyles: () => Record<string, string | string[]>;
}>;

// @public
export class ElementFixture {
    // Warning: (ae-forgotten-export) The symbol "ElementFixtureOptions" needs to be exported by the entry point index.d.ts
    constructor(options?: ElementFixtureOptions);
    // (undocumented)
    child: HTMLElement;
    // Warning: (ae-forgotten-export) The symbol "MockDocument" needs to be exported by the entry point index.d.ts
    //
    // (undocumented)
    document: MockDocument;
    // (undocumented)
    host: HTMLElement;
    // (undocumented)
    parent: HTMLElement;
    // (undocumented)
    superParent: HTMLElement;
    // Warning: (ae-forgotten-export) The symbol "MockWindow" needs to be exported by the entry point index.d.ts
    //
    // (undocumented)
    window: MockWindow;
}

// @public (undocumented)
export function emulateExecutionOfQwikFuncs(document: Document): void;

// @public (undocumented)
export function expectDOM(actual: Element, expected: string): Promise<void>;

// Warning: (ae-forgotten-export) The symbol "TestPlatform" needs to be exported by the entry point index.d.ts
//
// @public (undocumented)
export function getTestPlatform(): TestPlatform;

// @public (undocumented)
export function ssrRenderToDom(jsx: JSXOutput, opts?: {
    debug?: boolean;
    oldSSR?: boolean;
    raw?: boolean;
}): Promise<{
    container: _DomContainer;
    document: Document;
    vNode: _VNode;
    getStyles: () => Record<string, string | string[]>;
}>;

// @public
export function trigger(root: Element, queryOrElement: string | Element | keyof HTMLElementTagNameMap | null, eventNameCamel: string, eventPayload?: any): Promise<void>;

// @public (undocumented)
export function vnode_fromJSX(jsx: JSXOutput): {
    vParent: _ElementVNode;
    vNode: _VNode | null;
    document: _QDocument;
};

// @public (undocumented)
export function walkJSX(jsx: JSXOutput, apply: {
    enter: (jsx: JSXNode) => void;
    leave: (jsx: JSXNode) => void;
    text: (text: _Stringifiable) => void;
}): void;

// (No @packageDocumentation comment for this package)

```