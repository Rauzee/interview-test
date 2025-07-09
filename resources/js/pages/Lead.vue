<script setup lang="ts">
import { Button } from '@/components/ui/button';
import { Input } from '@/components/ui/input';
import { Label } from '@/components/ui/label';
</script>

<template>
    <div class="flex min-h-svh flex-col items-center justify-center gap-6 bg-background p-6 md:p-10">
        <div class="w-full max-w-sm">
            <div class="flex flex-col gap-8">
                <div class="flex flex-col gap-4">
                    <div>
                        <h1 class="text-xl font-medium">Cadastrar Lead</h1>
                    </div>
                </div>

                <form class="flex flex-col gap-6">
                    <div class="grid gap-6">
                        <div class="grid gap-2">
                            <Label for="name">Nome</Label>
                            <Input id="name" type="text" placeholder="John Doe" />
                        </div>

                        <div class="grid gap-2">
                            <Label for="email">E-mail</Label>
                            <Input id="email" type="email" placeholder="email@example.com" />
                        </div>

                        <div class="grid gap-2">
                            <Label for="phone">Telefone</Label>
                            <Input id="phone" type="tel" placeholder="(11) 99999-9999" />
                        </div>

                        <Button type="submit" class="mt-4 w-full">
                            Salvar
                        </Button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>
