# Workflow Analysis for FileSystem MCP Server Workflow

## Description
This workflow implements a secure Model Context Protocol (MCP) server that allows connected clients or AI agents to interact with a Linux file system by listing, creating, searching, reading, and writing files and directories — all while preventing arbitrary command execution for safety.

## Input Details
The workflow is triggered either by an MCP client via a webhook (MCP Server Trigger) or by another workflow invoking it with specific operation instructions (like read or write files).

## Process Summary
The workflow starts with an MCP server trigger that routes requests to various file system tools. It provides capabilities to list directories, create directories, and search for files using safe, parameterized shell commands. For more complex operations like reading or writing files, it uses internal workflow tools that accept filenames and contents as inputs. A switch node routes the execution to the appropriate command based on the requested operation (read vs. write). All file operations are scoped under the /home/node/ project root for security.

## Output Details
The workflow executes file system operations as instructed and returns the results (e.g., file contents or confirmation of file creation) back to the calling MCP client or parent workflow.

## Tags
MCP, file system, automation, n8n, secure commands, AI agent, Linux, workflow tool, production-ready
